---
title: "训练AI卢"
date: 2023-12-09T22:35:05+08:00
# weight: 1
# aliases: ["/first"]
tags: ["AI"]
author: "0x6c79"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "克隆卢的声音"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/super-duper-lamp/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---

- 训练使用[so-vits-svc-fork](https://github.com/voicepaw/so-vits-svc-fork)
- 训练集来自卢直播428：被封锁的涩谷
- 人声分离（去除BGM）使用[vocal remover](https://github.com/tsurumeso/vocal-remover)

克隆仓库到本地

```bash
git clone so-vites-svc-fork
cd so-vites-svc-fork
```

创建虚拟环境

```python
python -m venv venv
```

激活虚拟环境

```bash
source venv/bin/activate
mkdir dataset_raw dataset_raw_raw
```

安装依赖

```python
#install pytorch
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.6

#install so-vites-svc-fork
pip install -U so-vits-svc-fork

pip install pyannote-audio
```

分割数据集

```bash
git clone https://github.com/tsurumeso/vocal-remover.git
#从git克隆的仓库中没有作者训练好的模型，需要在release里下载压缩包，把models文件夹里的baseline.pth复制过来
cd vocal-remover
pip install -r requirements.txt
mkdir input_audio
mv path/to/an/audio/file input_audio
python inference.py --input input_audio/audiofile --gpu 0
mv audiofile.wave ../dataset_raw_raw/

cd ../
svc pre-split
```

训练数据集

```python
svc pre-resample
svc pre-config
svc pre-hubert
svc train -t
```
