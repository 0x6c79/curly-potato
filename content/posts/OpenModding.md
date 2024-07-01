---
title: "OpenModding"
date: 2023-12-09T20:41:24+08:00
# weight: 1
# aliases: ["/first"]
tags: ["TES","Mods","Gaming"]
author: "0x6c79"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
description: "A mirror about Wrye's Open Modding note."
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

## Wrye Notes: Open Modding

## 注：本文中的我指的是原文作者Wrye

**_In this paper, I discuss the idea of open modding – what it is and how best it can be achieved for the Morrowind community. Unfortunately, I'm being pulled back into real life, and so am unable to complete this document or have much time to discuss it. However, I hope that it will serve as a starting point for others with similar desires._**

***在这篇文章中，我讨论了开放模组制作的想法 - 它是什么以及它能使晨风社区达到多好的结果。很不幸，我正在被拉回现实生活，因此我不能完成这个文档或者有很多时间讨论它。然而，我希望它能作为一个为其他有类似愿望的人的起点***

## Contents

•  [Cathedral vs. Parlor](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#CathedralvsParlor)

•  [LGNPC Seyda Neen Redraft and Amulet of Scrye](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#LGNPCSeydaNeenRedraftandAmuletofScrye)

•  [Contrasts and Consequences](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#ContrastsandConsequences)

•  [Open Distribution](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OpenDistribution)

•  [No Takebacks](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#NoTakebacks)

•  [Open and Openable Distribution](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OpenandOpenableDistribution)

•  [Open Modification](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OpenModification)

•  [Levels of Modification](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#LevelsofModification)

•  [Modification Examples](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#ModificationExamples)

•  [Modification by Patch](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#ModificationbyPatch)

•  [Pervasive vs. Focussed Mods](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#PervasivevsFocussedMods)

•  [Open Modding License](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OpenModdingLicense)

•  [Basic Deal](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#BasicDeal)

•  [Details](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Details)

•  [Open Modification vs. Open Distribution](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OpenModificationvsOpenDistribution)

•  [Other Mechanisms](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#OtherMechanisms)

•  [General Behavior](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#GeneralBehavior)

•  [Users](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Users)

•  [Modders](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Modders)

•  [Distributors](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Distributors)

•  [Postscript](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Postscript)

•  [Reuse and Credits](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#ReuseandCredits)

•  [Credits](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Credits)

•  [License](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#License)

•  [Contact](https://wryemusings.com/Cathedral%20vs.%20Parlor.html#Contact)

## Cathedral vs. Parlor
## 大教堂 vs 客厅

There are essentially two ways that modders view the place of their creations in the modding community: The **_Cathedral_** view, and the **_Parlor_** view.

模组制作者看待他们的创作在模组社区中的位置基本上有两种方式：**大教堂**观点和**客厅**观点

In the **_Cathedral_** view, modding is viewed as being like a **_joint effort to build a cathedral._** Individually, our contributions may be small – and may not be worth doing for themselves. But by each person contributing something, we construct something larger and more worthwhile than any of us could do on our own. Under this view, creations are contributions – and may not be taken back. (Just as in building a Cathedral, it would not be allowed for a person to contribute a stained glass window and then later take it back.)

在**大教堂**观点中，模组制作被看作***一个共同努力建造一座大教堂***的过程。个体来说，我们的贡献可能很小 - 并且也许不值得为他们自己做。但通过每一个人贡献的一点，我们建造了比我们任何一个人能做到的更有价值、更大的东西。在这种观点之下，创作就是贡献 - 并且可能不会被收回。（就像正在建立一座大教堂，它不允许一个人贡献一个染色的玻璃窗之后再把它拿回去。

The **_Parlor_** view in contrast, is the view that mods are more like **_privately owned works of art displayed in the modder's parlor._** The modder invites others into the parlor to appreciate and enjoy the work of art – but may at any time close the parlor door and ask their guests to leave. And of course, the modder may be very selective about who they invite into their parlor. Under this view, our creations are never contributions; rather we continue to own and control them – takebacks are normal and accepted.

相比之下，在***客厅***观点中模组更像***模组制作者客厅中的私有艺术品***。模组制作者邀请其他人进入客厅来欣赏和享受这些艺术品 - 但可能随时关闭客厅的门并要求客人离开。当然，模组制作者也可能对邀请谁进入他们的客厅非常挑剔。在这种观点下，我们的创作从来都不是贡献；相比我们继续拥有和控制它们 - 收回是正常和可接受的。

The Parlor view allows the creator to retain complete control of their work. But the Cathedral view creates a much larger, more enduring and more perfected body of work – and for that reason, I prefer it.

客厅观点允许创作者保有对他们作品的完整控制权。但大教堂观点创造一个更大、更持久和更完美的作品体系 - 因此，我更倾向它。

### LGNPC Seyda Neen Redraft and Amulet of Scrye

To give an example... A year or two ago, Joe Stevens wrote a mod called "Less Generic NPC Seyda Neen", which fleshed out many of the characters in Seyda Neen by giving them non-generic responses to standard dialog topics. Joe eventually left the community, but another team took up the idea after him – creating LGNPC mods for a number of towns. But, after doing several towns, the LGNPC team had raised the bar considerably, and Joe's original work was looking pretty first draftish. At that point, I volunteered to redraft LGNPC Seyda Neen – fixing grammar, paragraph structure, logical inconsistencies and generally bringing it up to the current LGNPC bar.

举一个例子...一年或者两年以前，Joe Stevens写了一个叫做“Less Generic NPC Seyda Neen"的模组，此模组通过给他们（NPC）对标准对话主题的非通用响应从而充实了许多Seyda Neen中的角色。Joe最终离开了社区，但其他团队在他之后继承了这个想法 - 为一些城镇创造LGNPC模组。但是，做了几个城镇之后，LGNPC 团队大大提高了标准，Joe的原始作品看起来就相当像初稿。在那时，我自愿的翻新了LGNPC Seyda Neen - 修复语法、段落结构、逻辑不一致等问题，并总体上让它达到当前的LGNPC标准。

By the Cathedral view, my redraft was a good thing – I took something that was good and made it even better. And as a result, Joe's original work is seen and appreciated more then before.

从大教堂观点来看，我翻新模组是一件好事 - 我拿了一些好东西并把它做的更好。结果来说，Joe的原始作品比以前更受关注和欣赏。

But by the Parlor view, my redraft was a bad thing, since I changed Joe's original work. According to the parlor view, I should have created a new LGNPC Seyda Neen from scratch. The result of this would have been two competing LGNPC Seyda Neen's. Not only would this have been a lot more work, but if mine were substantially better, it would have crowded out Joe's original – thus ensuring that even fewer people saw it.

从客厅观点来看，我翻新模组是一件坏事，因为我更改了Joe的原始作品。按照客厅观点，我应该从头创造一个新的LGNPC Seyda Neen。这不止会增加许多工作量，而且如果我的在实质上更好，它将会把Joe的原始作品挤掉 - 由此确保更少的人看见它。

Fortunately for all of us, Joe himself was more of a Cathedral sort of guy and had already given the LGNPC team permission to edit and redistribute his work. Hence, my edit had been pre-blessed.

对我们来说幸运的是，Joe本人更像大教堂这类的人并且已经给了LGNPC团队编辑和重新分发他作品的授权。因此，我的编辑已经得到了提前的祝福。

However, not everything turned out perfectly. In my revision of Seyda Neen, I have the bard tell a ghost story related to one of my favorite mods: Ivza's Amulet of Scrye. If the player doesn't have Amulet of Scrye, then the ghost story is just an extra bit of non-generic dialog. But if the player does have AoS, then ghost story compliments it nicely, emphasizing the spookiness of that mod. However, a few weeks after I released the LGNPC Seyda Neen, Ivza decided to pull Amulet of Scrye from public distribution. To me, that felt like the glazier coming into the Cathedral, pulling out the stained glass window that he had put in earlier, and taking it home with him. But for Ivza, I think that it was just a closing of his parlor door.

然而，并非一切都完美。在我对Seyda Neen修订时，我做了一个吟游诗人讲述一个与我最喜欢的模组相关的鬼故事：Ivza的Amulet of Scrye。如果玩家没有Amulet of Scrye模组，那么这个鬼故事仅仅是一个额外的非通用对话。但如果玩家有Amulet of Scrye模组，那么鬼故事很好的赞美了它，强调那个模组的阴森恐怖。然而，在我发布了LGNPC Seyda Neen几周后，Ivza决定从公共发行中收回Amulet of Scrye模组。对我来说，那就像玻璃工走进大教堂，把他之前安好的彩色玻璃窗拉出来，然后带回家。但对Ivza来说，我认为那只是关上了他客厅的门。

It was this, combined with very vocal support for the parlor view on the forum, that led me to retire. I had several ongoing projects and there were several items that I would have liked to continue working on, but it seems like the Parlor view is predominant – and personally I don't find it that inspiring.

就是这样，结合着在论坛上非常强烈的支持客厅观点的声音，使得我退出。我有几个正在进行的项目并且有几个我想要继续做的东西，但看起来客厅观点占了主导地位 - 就我个人而言我不认为它有那么鼓舞人心。
### Contrasts and Consequences
### 对比和结果

#### Modding is a Joint Effort
#### 模组制作是共同努力

Almost all of Morrowind modding is a group effort to one degree or another. There are very few mods that do not owe huge debts to earlier produced mods and/or to the expertise and tools provided by earlier modders.

几乎所有晨风的模组制作在某种程度上都是集体努力的结果。很少有模组不欠早期制作的模组和/或早期模组作者提供的专业知识和工具的巨大帮助。

#### New Work vs. Duplication 新作品 vs 重复作品

The Cathedral view vastly reduces duplication of effort – instead promoting either improvements in, or extensions of the original, or the creation of entirely new, complementary works. One doesn't have go far in reviewing one's mod library to see quite a few of these examples of mods that extend or fix earlier mods. E.g.: LGNPC, Adventure, Join All Houses, CharGen, Inferno's Island, Kivan's patches, alchemy sorters, etc.

大教堂观点极大地减少了重复用功 - 取而代之促进对原作品的改进或扩展，或创造一个全新的、互补的作品。人们无需深入审查自己的模组库，就能看到相当多的扩展或修复之前模组的例子。例如：LGNPC, Adventure, Join All Houses, CharGen, Inferno's Island, Kivan's patches, alchemy sorters等。

#### Perfection vs. Stagnation
#### 完美 vs 停滞

The Cathedral view tends towards perfection, while the Parlor view tends towards repetition and stagnation. **_Repetition,_** because earlier useful works that have been closed off have to be recreated. **_Stagnation,_** because this fails to lead to improvements, and more importantly because few modders are interested in replicating something that has already been done before. (Especially since, if they knew of the original, they probably have a copy of the original mod, and hence have no personal need to recreate it.

大教堂观点趋向完美，然而客厅观点趋向重复和停滞。**重复**，因为之前被关闭的有用作品必须重新创作。**停滞**，因为这无法带来改进，并且更重要的是因为很少有模组制作者有兴趣复制之前已经有的东西。（特别是因为，如果他们知道原模组，他们可能已经有了原模组的拷贝，因此没人需要重新创造它）。
#### Integration vs. Isolation
#### 集成 vs 隔离

The Cathedral view tends towards rich integration between mods. But under the Parlor view, there's not much point of integrating with another mod – since that mod can be removed at any time. Certainly, I would not have added the Amulet of Scrye references to LGNPC Seyda Neen, if I had thought Ivza might remove it.

大教堂观点趋向在模组之间丰富的集成。但在客厅观点下，与其他模组的集成没有意义 - 因为模组可以随时移除。当然，如果我认为Ivza可能会删除它，我就不会添加对Amulet of Scrye的引用。

#### Authorial Longetivity
#### 作者寿命

Improved works are much more likely to give everyone credit. OTOH, if two works are independently created to do the same job, then it's likely that only one of them will "win" (i.e. be widely known/used) – and thus the effort and name of the loser will be lost. In competitions, there's little desire to mention your competitor in your readme; but in extensions and improvements, the norm is for the original author to get top billing.

改进的作品更有可能给每个人带来荣誉。反过来说，如果两个作品是独立创造的并且做的是相同的事，那么很可能只有一个会“赢”（比如被广泛认识的/使用的）- 并且因此失败者的努力和名誉都会消失。竞争中，几乎没有人会在自己的自述文件中提及对手；但扩展和改进，原作者得到了最高的评价却是常态。

#### Cathedral Effect
#### 大教堂效应

Many modders (such as myself) aren't interested in working in a non-Cathedral community. It's belonging to a community, creating something that outlasts our own efforts, that integrates and grows even when we're away that makes the community so interesting. But under the Parlor view, much of what has been built in the past just disappears.

很多模组制作者（例如我自己）对在非大教堂社区工作不感兴趣。它属于社区，创造出比我们自己的努力更长久的东西，即使我们不在，它也会融合和成长，这使得社区变得如此有趣。但在客厅观点下，许多在过去创造的东西都消失了。

Morrowind players and modders are already paying the price for the lack of prior action to support the Cathedral view. The loss of previous modding sites (Morrowind Files, Euro-Morrowind, Gamer's Roam, etc.) has meant the loss of many of the mods originally on those sites. Many of these mods are still available on people's hard disks, but without a clear re-uploading agreement, these have not been added onto new download sites. (Much of the recent dispute on the forum was on the topic of when and if these could ever be re-uploaded to new sites.)

晨风玩家和模组制作者已经为缺少先前的行动支持大教堂观点而付出了代价。以前的模组网站丢失（Morrowind Files, Euro-Morrowind, Gamer's Roam等）意味着失去了原来在这些网站上的许多模组。许多这样的模组仍然在人们的硬盘里，但没有一个清晰的重新上传的许可，这些模组就不能添加到新的下载网站中。（最近许多在论坛上的争论都是关于什么时候和如果他们能重新上传到新的网站上的话题。）

Aside from just these lost files, other creations would likely have not been withdrawn if there were clear community standards and processes in support of the Cathedral view. I.e., if all upload and link sites had "no takebacks" policies, more of the old mods would be under no takeback licenses, and so could not have been removed.

除了这些失去的文件外，如果有清晰的社区标准和流程来支持大教堂观点，其他的创造可能不会被撤回。例如，如果网站对所有的上传和链接没有收回政策，更多的旧模组将处于不收回许可证下，因此也就不会被移除。

## Open Distribution
## 开放分发

Okay, enough about the problem. Now, what can/should be done about it? I see two main questions: 1) What does the Cathedral view mean in practice? and 2) How can/should the Cathedral view be promoted?

好吧，关于问题说的够多了。现在，有什么能/应该做的呢？我看见了两个主要问题：1) 大教堂观点在实践中意味着什么？2) 怎么能推广大教堂观点呢？

### No Takebacks
### 不取回

At it's minimum, the Cathedral view means, "No takebacks!" Once a mod has been released to the public, then it can't be taken back. Okay, sounds good, but... 1) What about group mods? 2) What does "released to the public" mean? Does email count? How about a sharing through a Yahoo briefcase? 3) Can the modder still restrict distribution to their own personal site? Can they require registration? These questions be discussed in the next section.

至少来说，大教堂观点意味着“不取回！” 一旦一个模组向公共发行，他就不能被取回。好吧，听起来不错，但是... 1) 那么一组模组呢？ 2) “向公共发布“是什么意思呢？电子邮件算吗？通过雅虎公文包分享的怎么样呢？ 3) 模组作者还能限制分发在他们自己的网站上吗？他们需要注册吗？ 这些问题将在下个区域讨论。

At a more advanced level, the Cathedral view often means that others can modify the original mod. There are clearly arguments for this (the perfection and integration described above), but there is also a strong argument against it (artistic vision of the original modder). These issues will be discussed later.

更深层的来说，大教堂观点通常意味着其他人能修改原模组。对此有明确的论据（上文的[[#Perfection vs. Stagnation]]和[[#Integration vs. Isolation]]中进行了描述），但也有一个强烈的论据反对它（原模组作者的艺术视野）。这些问题将在后面讨论。

### Open and Openable Distribution
### 开放和可开放分发

The most basic level (the "foundation" you might say) of the Cathedral view is: "No takebacks!" One way of achieving this is to simply say that once a mod has been released, that it is **_Open Distribution_** – i.e., **_anyone else can distribute it with no additional permission required from the author._**

大教堂观点的最基本的层次（你也许会说“基石”）是：“不取回！” 达成此的一个方法是简单地说模组一旦发布，它就是**开放分发** - 例如，**任何人都能分发它而不要原作者的附加许可**。

However, there are a lot of modders who are willing to keep their mods available, but prefer to have them served by a single website. For these modders, and **_Openable Distribution_** might be solution. Openable Distribution allows the modder to limit distribution to preferred web sites – so long as at least one such website is available. As soon as that website goes down for an appreciable period of time (a week), then the mod becomes Open Distribution.

然而，有很多模组作者愿意保持他们的模组可用，但倾向于在单一网站上保有他们。对这些模组作者来说，**可开放分发**可能是解决方案。可开放分发允许模组作者限制分发到倾向的网站 -

There are several benefits to Openable Distribution:

•  **_Management:_** For a creator, mod distribution through a personal website is the easiest to manage by far: no hoops to jump through, no waiting for other people to check in their upload. Personally, I've created and uploaded mods in the space of an hour to answer forum questions, and I've uploaded 14 versions of my Mash utility in as many days. That sort of speed and responsiveness could not have been achieved if I had been serving my mods through one of the major web sites. Mega Mods (TCs, LGNPC) also often benefit greatly from dedicated web sites for distribution and management.

•  **_Artistic Reward:_** Mod users tend to be quite sparing in their applause. Hence, the only really reliable measure of success is the download counter provided by the download site and/or the site stats pages for your personal web site – such stats are easiest to monitor when the mod is only available from one site. In addition, personal download sites allow the modder to express personality and artistic vision and advertise their other mods. See for example [Silaria's Morrowind Visions](http://www.morrowindvisions.com/MWVisions_Clothing.htm).

The only care that needs to be exercised with Openable Distribution, is that it not be used as a cover for non-open distribution. I.e., the amount of downtime for the the preferred distribution site cannot be either prolonged or frequent. E.g., the site should not be down for more than a week at a time, nor down for more then 7 days in a month.

#### Public Release

I would take _public release_ to mean release to anyone other than the mod creators/beta testers – by any mechanism (even email). Obviously, neither "creators" nor "beta testers" definitions should be bent in an effort to limit distribution. Basically, as soon as anyone whose major intent is just to enjoy the mod is given a copy of the mod, then the mod has been released.

#### Access Registration

I'm fairly sure that it should be part of both Open and Openable Distribution definitions that downloading the mod not require any sort of registration – except for adult content mods – which may require a registration of sufficient age to access adult materials.

However, several major download sites require registration as part of the commercial operation. (E.g., Morrowind Summit.) So perhaps this should be allowed also. However, I think that downloads from personal web sites should **_not_** require registration – this seems like a form of restriction on downloading.

## Open Modification

**_Open Modification_** means that the mod author allows their mod to be modified and redistributed at will. In the software open source community, this is one of the defining characteristics of "open source". However, the modding world is different from the world of practical software, and the desirability of Open Modification is much more debatable for mods. I'll discuss some of these considerations below, but in the end, **_I think that whether a mod is Open Modification, or partially open to modification, or not modifiable at all should largely be left up to the mod author._**

### Levels of Modification

Before getting into the pros and the cons of open distribution, it's useful to consider the levels of modifications that can be made to a mod.

#### Error Correction

•  GMST removal. Fix typos, grammar, etc.

•  Fix logic errors that break quests, etc.

#### Compatibility Patch

•  Fixing things that aren't errors in themselves, but which cause or are vulnerable to compatibility errors.

#### Standardization

•  Dialog standardization. "continue" to "Continue", etc.

•  Object names. (E.g. to follow Wrye Patches naming standards)

#### Re-drafting

•  Taking what is clearly an early draft and redrafting it, but sticking to the original author's intent as much as possible.

•  However, redrafting necessarily involves some degree of artistic interpretation.

#### Extension

•  Adding new material that is consistent with the original mod.

#### Multi-pathing

•  Allowing the user to take a different path, with different consequences than the original mod. I.e., the original path is left intact and is not diminished, but the user is given a chance to take a different path.

•  However, the multi-pathing is not to the degree that it perverts the intent of the original mod.

•  For example: in Inferno's Island Revisited, you're forced to kill two members of the Blades in order to continue the main quest. Multi-pathing would allow you to avoid this (after all, if you follow Morrowind's main story line, you **_are_** a Blade!)

#### Artistic Conflict Resolution

•  Correcting artistic conflicts between mods.

•  E.g., for LGNPC Seyda Neen, moving the Bal Molagmer "Forged Land Deed" quest from Indrele to someone else to resolve conflict.

•  E.g., removing Drakron's French Maid vendor from Six Fishes because her outfit is anachronistic there.

#### Artistic Destruction

•  Removing some element of the mod for the intent of changing the artistic intent of the mod.

•  E.g., removing the unicorn and fairies from Korana's Magus Realm mod.

#### Perversion

•  Modifying the mod in such a way that the mod's artistic intent is perverted – i.e., the original artistic intent is actually attacked in the modification.

•  E.g., taking the models from a Mog mod and using them in a Mog Hunters mod.

•  E.g., adding Moogles to Qarl's Underground, and having Qarl's NPCs say things like, "Moogles are the best!"

### Modification Examples

To make the levels of modification more concrete, here are some real life examples that I'm familiar with.

#### LGNPC Seyda Neen

•  Change Completed

•  Error correction.

•  Re-drafting

•  Mild extension.

•  Possible Changes

•  More extension, maybe substantial extension.

#### Wrye World Clothing Mods

•  I produce alternate versions of original esps. I.e., the user still has to download the original mod, but then they (usually) use my esp in place of the original esp. My esp is a modified version of the original esp.

•  Changes Completed

•  Error correction

•  Extension (add clothes to Erika + related dialog)

•  Deletion for:

•  Removing cheap solutions that are no longer necessary (dump crates)

•  Resolving artistic conflict (removing French Maid vendor from Six Fishes)

•  French Maid outfit is anachronistic in game – especially in that location, and Drakron did not have a lot of artistic intent invested in her.

#### LCV (Living Cities of Vvardenfell)

•  Possible Changes

•  Extension to other cities.

•  Resolve story conflicts with LGNPC mods.

#### Inferno's Island Revisited

•  Possible Changes

•  Error corrections.

?  Redrafting. Existing dialog is pretty minimal.

•  Multi-pathing. Allow not killing Blades agents, etc.

#### Korana Magus Realm

•  Possible Changes

•  Artistic Deletion: Get rid of unicorn and fairies! (Love the tower and realm, but not so fond of cutesy animals.)

### Modification by Patch

It's possible to modify a mod while still leaving the original intact by either releasing either an alternative or patch esp.

A patch esp is probably preferable if the original esp is large and/or likely to change. It also leaves a clear distinction in the users mind between the original mod and the patch. And as a practical consequence, it simplifies support issues for the original modder – since the original and patch are clearly separate.

OTOH, an alternative esp is necessary if the modifier wants to change the placement of refs. Alternative esps also have the advantage of reducing the user's esp count, and thus makes their mod management easier.

In considering what counts as "modification" for the purposes of licensing, one could argue either that both patch and alternate esps count as modifications, or that neither esp counts as modification. I'll split the difference, and say that an alternate esp is a modification, while a patch esp is not.

### Pervasive vs. Focussed Mods

It's useful to distinguish pervasive mods from focussed mods. Focussed mods typically add new areas and quests to the game, but don't change the existing gameplay. I.e., if a focussed mod is removed, you only notice it's absence in that the specific areas and people that it adds are no longer there. Pervasive mods on the other hand change the gameplay in a fairly pervasive way. If pervasive mods are removed, their absence is felt through the entire game.

Tribunal and Bloodmoon are primarily focussed mods. OTOH, Wakim's Game Improvements, Srikandi's Alchemy, Better Bodies are all examples of pervasive mods. Other mods have both elements: Ivza's Amulet of Scrye had a series of quests, but it also had a placement of random ghosts throughout the world that affected the general atmosphere of the game.

While focussed mods can benefit from Open Modification, Open Modification seems most advantageous and desirable for pervasive mods. Ivza's Amulet of Scrye is a good example of this. There are a lot of tomb raiding, necromancy and magic mods – Amulet of Scrye impacts the gameplay of all those other mods. Hence, theres more of a desire to patch or integrate with Ivza's mod than with a mod that takes you off to some island.

## Open Modding License

As discussed above, the foundation of the Cathedral view is "no takebacks" – i.e., either Open Distribution or Openable Distribution licenses for mods. At a more advanced level, the Cathedral view means a license that allows at least some degree of Open Modification. Several such licenses have been proposed.

However, the problem with these licenses is that they do nothing to _encourage,_ a modder to use one of their licenses. I.e. the modder gains no benefit for adding one and suffers no penalty for not adding one. True, at least some modders will add one anyway – but I strongly suspect that most will not.

What is needed is a license that does a little arm twisting. If this seems a little negative to you, consider that open source licenses do exactly the same thing – and doing so has been crucial to the success of open source software.

### Basic Deal

The basic deal of the OML would be: **_I (the creator of this mod) will allow you (the end user) to use my mod, if you agree that any mods that you produce and distribute will be at least Openable Distribution. If you do not agree to these terms, then not only may you not use my mod, but you may not keep a copy of this mod._**

So, what's that mean? 1) If you never produce any mods, or only produce mods that you never distribute, then you're never limited by this agreement – enjoy! 2) But if you produce a mod and distribute it (i.e., give it to anyone other than yourself), then you're bound by the terms of the agreement and your mod must be at least Openable Distribution. 3) If you don't agree to the terms then you may not use any OML mods, and moreover, you must remove any OML mods from your hard disk, personal web site, Yahoo briefcase, etc.)

There's one out in this agreement. If you use an OML mod, and have not distributed a mod yet, but later decide to do so – but at that time decide to non Openable Distribute it, then you can do so – but you'll first need to remove all OML mods from your hard disk, Yahoo briefcase, etc.

However, this out will **_not_** be available if you have otherwise agreed that all of your mods will be Open Distribution. E.g., suppose that there is an "Open Distribution" thread in which people post their agreement that all of their past and future mods are Open Distribution. (I'm considering requiring that users make such a posting as a condition to my providing help for my mods.)

If you already have mods released, then you will not be able to use or keep OML mods unless all of your distributed mods are made Open Distribution.

Note that this agreement applies if you distribute your mod to anyone other than yourself. I.e., even if you email it, or pass it along in some other private matter, that still counts as distribution.

### Details

#### Contained Mods

Suppose that your mod contains a mod that is not Open Distribution – i.e., the creator of that mod has placed restrictions on how you may distribute your mod. Frankly, I don't know of a case where this is true, but if it is true – the agreement **_still applies._** I.e., if your mod is not Open Distribution, then you cannot use use OML licensed mods.

#### Group Mods

Suppose that a mod is produced by a group. In this case, the team leader is still bound fully by the terms of the agreement. Also, the contributions by any team member using OML mods are also considered to be Openable Distribution. (So, if all team members are OML users, then the team product is automatically Openable Distribution.)

#### Clear Licensing

In distributing your mod, then the main readme must include an explicit Openable Distribution license, or a statement that it is released under an Openable Distribution license which is included in the distribution in a separate text or html file.

#### Notes

1) OML is Open Distribution, of course. 2) Though OML requires that the users distributed mods be Openable Distribution licensed, it does not require that they be OML licensed. 3) The license would cover mods and utilities for the Morrowind platform only. (I.e., not Oblivion or anything else.) 4) If the license is in conflict with the Bethesda EULA, then the Bethesda EULA take precedence of course in the areas of conflict. 5) Standard legal boilerplate regarding liability, etc.

### Open Modification vs. Open Distribution

As discussed above, Open Modification is often, but not always desirable. Hence, I think that there should probably be two versions of the OML license. The first (OML-A) would allow Open Modification, while the second (OML-B) would not. In addition, any modification to an OML-A licensed mod would also have to be released under an OML-A license. Other than that, the licenses would be pretty much the same – i.e., they would only require that users release their code as Openable Distribution.

#### Limits on Modification

If an OML-B mod is distributed, then it must be redistributed with all readme and licenses. It may be broken up into several parts (for downloading convenience for large mods), and it may be recompressed into a different format (e.g., zip to rar). However, if it is broken up, then the read me and license must be included with each part.

### Other Mechanisms

Aside from the Open Modding license, a couple of other mechanisms are possible to help promote the Cathedral model.

#### Help Requirements

Before providing help on a released mod, the mod's creator might require that users agree (irrevocably) to make all of the user's past and future mods Open Distribution.

#### Replacement Mods

Another option would be to create open versions of non-open mods. E.g., if the author of a mod refuses to open it, yet it implements a good and generally useful idea, then someone might decide to create an open version of the mod. Part of the benefit of this approach is that just the threat of it may be sufficient to encourage the original modder to open his mod. (Note that this sort of approach would likely only work when the original mod is relatively simple. E.g., an invisible armor mod.)

#### License Status Database

It would be good to have a central database listing all(?!) mods and their license status. Naturally it would be important that people putting data into the database be reliable, and that the database be shared.

## General Behavior

Here are some additional rules of thumb designed to encourage open modding and a generally pleasant modding atmosphere.

### Users

#### Gratitude

•  Show some gratitude to the mod authors once in a while!

### Modders

#### License and Readme

•  Release your mod under the most open license that you feel comfortable with. **_At the least,_** release it under an Openable Distribution license.

•  Strongly consider using a OML license, which encourages other modders to also release Open Distribution mods.

•  If your work is a modification of an existing work, or if it includes components which are non-modifiable (because they come from another author), be sure to take this into consideration in selecting your license.

#### Readme

•  Provide your readme in html format, and at the top, and place links to any relevant feedback and/or applause forum topics. If you only want to hear positive applause, be sure to make this clear.

•  If the mod is a modification or an existing mod, be sure to give full authorial credit to the original author. This typically means listing them first in the mods "Author" box, and listing them first (with full explanation of their original product) in your readme.

•  Likewise, if your mod contains components from other mods, be sure to give those authors full credit. And if the license agreement covering those components of the mod is different from the license covering your original work, be sure to be very clear about which components are theirs – and thus under their license.

#### Support and Applause Topics

•  Create a forum topic for discussion of your mod.

•  If there's a forum that hosts applause topics, you may want to add a topic for yourself there.

#### Ignore Idiots

•  If you can't stand hearing from idiots who do nothing but criticize, complain and demand, then ignore them...

•  Use forum "Ignore" features if available (Elder Scrolls for one provides this).

•  In the extreme, put support on a forum that allows you to limit idiots more strongly. Note that "no takebacks" does NOT say that you have to support your mod or deal with idiots.

### Distributors

#### Mod Backup and Open Distribution Mod Hosting

•  Keep backups of Openable (or better) Distribution mods from other download sites and personal sites in case those sites go down.

•  If the original site goes down, or goes down frequently, check with the author first to see if the problem can be resolved. If not, make the mod available from your site.

#### Upload Requirements

•  Require that all mods uploaded to your site have at least an Openable Distribution license, and that the license be included or referred to in the readme. If it's only referred to in the readme, then the upload zip must also contain a copy of the license agreement.

•  Strongly suggest that uploaders use one of the standard licenses.

#### Downloading

•  When listing mods, indicate the type of license that it's distributed under.

•  For mods with standard licenses, provide links from mod license type to a copy of the mod license.

## Postscript

While many people have been supportive of the Cathedral ideal, very few people have supported the OML. I have recently been looking at other licensing options. Results of that investigation can be found at [UESP Wiki: Licensing](http://www.uesp.net/wiki/index.php?title=Tes3Mod:Licensing). Since I was dissatisfied with the available options, I've devised my own informal licenses ([Wrye Modding Licenses 1.0](https://wryemusings.com/WML%201.0.html)). While these are not as aggressive as the OML, it is hoped that providing standard licenses (especially licenses with Share Alike attributes) will help to open the community up somewhat.

## Reuse and Credits

### Credits

•  (C) 2005, by Wrye

### License

•  Feel free to mirror this.

### Contact

•  Home page: [Wrye Morrowind](http://wrye.ufrealms.net/)

•  Best way to contact me is by PM to "Wrye" at the Elder Scrolls forum.



## 原链接

> https://wryemusings.com/Cathedral%20vs.%20Parlor.html
