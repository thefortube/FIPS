---
fip: 0
title: FIP Purpose and Guidelines
status: Implemented
author: ForTube Community
discussions-to: https://forum.for.tube/
created: 2020-07-22
updated: 2020-09-03
---

## What is an FIP?

FIP stands for ForTube Improvement Proposal, it has been adapted from the SIP (Synthetix Improvement Proposal). The purpose of this process is to ensure changes to ForTube are transparent and well governed. An FIP is a design document providing information to the ForTube community about a proposed change to the system. The author is responsible for building consensus within the community and documenting dissenting opinions.

## FIP Rationale

We intend FIPs to be the primary mechanisms for proposing new features, collecting community input on an issue, and for documenting the design decisions for changes to ForTube. Because they are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.

It is highly recommended that a single FIP contain a single key proposal or new idea. The more focused the FIP, the more successful it is likely to be.

An FIP must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement.

## FIP Work Flow

Parties involved in the process are the *author*, the [*FIP editors*](#fip-editors), and the ForTube community.

:warning: Before you begin, vet your idea, this will save you time. Ask the ForTube community first if an idea is original to avoid wasting time on something that will be rejected based on prior research (searching the Internet does not always do the trick). It also helps to make sure the idea is applicable to the entire community and not just the author. Just because an idea sounds good to the author does not mean it will have the intend effect. The appropriate public forum to gauge interest around your FIP is [the unofficial ForTube Discord] or [the unofficial ForTube Telegram].

Your role as the champion is to write the FIP using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea. Following is the process that a successful FIP will move along:

```
Proposed -> Approved -> Implemented
  ^                     |
  +----> Rejected       +----> Moribund
  |
  +----> Withdrawn
  v
Deferred
```

Each status change is requested by the FIP author and reviewed by the FIP editors. Use a pull request to update the status. Please include a link to where people should continue discussing your FIP. The FIP editors will process these requests as per the conditions below.

* **Work in progress (WIP)** -- Once the champion has asked the ForTube community whether an idea has any chance of support, they will write a draft FIP as a [pull request]. Consider including an implementation if this will aid people in studying the FIP.
* **Proposed** If agreeable, FIP editor will assign the FIP a number (generally the issue or PR number related to the FIP) and merge your pull request. The FIP editor will not unreasonably deny an FIP. Proposed FIPs will be discussed on governance calls and in Discord. If there is a reasonable level of consensus around the change on the governance call the change will be moved to approved. If the change is contentious a vote of token holders may be held to resolve the issue or approval may be delayed until consensus is reached.
* **Approved** -- This FIP has passed community governance and is now being prioritised for development.
* **Implemented** -- This FIP has been implemented and deployed to mainnet.
* **Rejected** -- This FIP has failed to reach community consensus.
* **Withdrawn** -- This FIP has has been withdrawn by the author(s).
* **Deferred** -- This FIP is pending another FIP/some other change that should be bundled with it together.
* **Moribund** -- This FIP has been implemented and is now obsolete and requires no explicit replacement.

## What belongs in a successful FIP?

Each FIP should have the following parts:

- Preamble - RFC 822 style headers containing metadata about the FIP, including the FIP number, a short descriptive title (limited to a maximum of 44 characters), and the author details.
- Simple Summary - “If you can’t explain it simply, you don’t understand it well enough.” Provide a simplified and layman-accessible explanation of the FIP.
- Abstract - a short (~200 word) description of the technical issue being addressed.
- Motivation (*optional) - The motivation is critical for FIPs that want to change ForTube. It should clearly explain why the existing specification is inadequate to address the problem that the FIP solves. FIP submissions without sufficient motivation may be rejected outright.
- Specification - The technical specification should describe the syntax and semantics of any new feature.
- Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.
- Test Cases - Test cases may be added during the implementation phase but are required before implementation.
- Copyright Waiver - All FIPs must be in the public domain. See the bottom of this FIP for an example copyright waiver.

## FIP Formats and Templates

FIPs should be written in [markdown] format.
Image files should be included in a subdirectory of the `assets` folder for that FIP as follows: `assets/fip-X` (for fip **X**). When linking to an image in the FIP, use relative links such as `../assets/fip-X/image.png`.

## FIP Header Preamble

Each FIP must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order. Headers marked with "*" are optional and are described below. All other headers are required.

` fip:` <FIP number> (this is determined by the FIP editor)

` title:` <FIP title>

` author:` <a list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.>

` * discussions-to:` \<a url pointing to the official discussion thread at forum.for.tube\>

` status:` < WIP | PROPOSED | APPROVED | IMPLEMENTED >

` created:` <date created on>

` * updated:` <comma separated list of dates>

` * requires:` <FIP number(s)>

` * resolution:` \<a url pointing to the resolution of this FIP\>

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

#### `author` header

The `author` header optionally lists the names, email addresses or usernames of the authors/owners of the FIP. Those who prefer anonymity may use a username only, or a first name and a username. The format of the author header value must be:

> Random J. User &lt;address@dom.ain&gt;

or

> Random J. User (@username)

if the email address or GitHub username is included, and

> Random J. User

if the email address is not given.

#### `discussions-to` header

While an FIP is in WIP or Proposed status, a `discussions-to` header will indicate the URL at [forum.for.tube](https://forum.for.tube/) where the FIP is being discussed.

#### `created` header

The `created` header records the date that the FIP was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

#### `updated` header

The `updated` header records the date(s) when the FIP was updated with "substantial" changes. This header is only valid for FIPs of Draft and Active status.

#### `requires` header

FIPs may have a `requires` header, indicating the FIP numbers that this FIP depends on.

## Auxiliary Files

FIPs may include auxiliary files such as diagrams. Such files must be named FIP-XXXX-Y.ext, where “XXXX” is the FIP number, “Y” is a serial number (starting at 1), and “ext” is replaced by the actual file extension (e.g. “png”).

## FIP Editors

The current FIP editors are:

` * David Lei (@Master-LY)`

` * seamon (@seamon)`

` * Aaron (@aaronliug)`

` * Mirai (@Mingliang233)`

## FIP Editor Responsibilities

For each new FIP that comes in, an editor does the following:

- Read the FIP to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
- The title should accurately describe the content.
- Check the FIP for language (spelling, grammar, sentence structure, etc.), markup (Github flavored Markdown), code style

If the FIP isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the FIP is ready for the repository, the FIP editor will:

- Assign an FIP number (generally the PR number or, if preferred by the author, the Issue # if there was discussion in the Issues section of this repository about this FIP)

- Merge the corresponding pull request

- Send a message back to the FIP author with the next step.

The FIP editors monitor FIP changes, and correct any structure, grammar, spelling, or markup mistakes we see.

The editors don't pass judgment on FIPs. We merely do the administrative & editorial part.

## History

The FIP document was derived heavily from the SIP Synthetix Improvement Proposal document in many places text was simply copied and modified. Any comments about the FIP document should be directed to the FIP editors.

### Bibliography

[the unofficial ForTube Discord]: https://discord.com/invite/3AGgWxy
[the unofficial ForTube Telegram]: https://t.me/theforceprotocol666
[pull request]: https://github.com/thefortube/FIPS/pulls
[markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).




## 什么是FIP？

FIP是ForTube改进提案的缩写，它是从SIP（Synthetix改进提案）改进而来。FIP的目的，是确保ForTube的改进是透明的，并处于良好治理之下。FIP是一个设计文档，为ForTube社区提供有关系统改进提案的信息。FIP的作者负责在社区内建立共识，并记录不同意见。

## FIP的理论基础

我们希望FIP成为提出新功能、收集社区对某个问题的意见、以及记录关于ForTube改进的设计决策的主要机制。因为在版本库中，FIP以文本文件的格式进行维护，所以它们的修订历史记录，就是功能提案的历史记录。

强烈建议单个FIP包含单个关键提案，或新的想法。FIP越精炼，就越可能成功。

FIP必须满足某些最低标准。它必须清楚且完整地描述所提案的改进措施。改进措施必须代表纯粹的改进。


## FIP工作流程


参与该进程的各方包括FIP*作者*、[*FIP 编辑*](#fip-editors) 和 ForTube社区。

:warning:在开始之前，先审查一下你的想法，这样可以节省时间。首先咨询ForTube社区，你的想法是否属于原创，以避免浪费时间在一些在先前的研究中已被拒绝的提案上（互联网搜索并不总是有效）。这也有助于确保这个想法适用于整个社区，而不仅仅适用于作者。这个想法对作者来说也许是好的，但并不意味着它会产生预期的效果。可以在ForTube的[官方Discord群组](https://discord.com/invite/MYKm35s)进行公开讨论，以便验证你的提案是否能够引发兴趣。


你可以使用下面描述的风格和格式编写FIP，在论坛中适当的指导讨论，并围绕这个想法建立社区共识。成功的FIP将遵循以下流程：

```
Proposed -> Approved -> Implemented
  ^                     |
  +----> Rejected       +----> Moribund
  |
  +----> Withdrawn
  v
Deferred
```

以上每个状态的更改，都需要由FIP作者提出请求，并由FIP编辑进行审核。FIP作者需要提供一个链接，指向人们继续讨论该FIP的地址。

* **进行中（WIP）** --  一旦FIP作者咨询ForTube社区，其想法是否有获取支持的机会，他们会写一份FIP草案来[推动申请](https://github.com/ForTube-Protocol/FIPs/pulls)。请考虑在草案中包含实施计划，这将帮助人们了解该FIP。
* **已提交** -- 如果提案得到同意，FIP编辑将为该FIP分配一个编号（通常是与FIP相关的议题编号或PR编号），并合并您的提案请求。FIP编辑不会无故否决任何FIP。提案的FIP将在治理电话会议和Discord群组中进行讨论。如果在治理电话会议中，对于该提案达到了一定程度的共识，那么该提案将被批准。如果存在争议，治理代币持有人可进行投票来解决问题，或推迟批准直到达成共识。
* **已批准** -- 该FIP已经通过了社区治理核准，目前正在优先推进。
* **已实施** -- 该FIP已经实施，并部署到主网。
* **已驳回** -- 该FIP未能达成社区共识。
* **已撤回** -- 该FIP已被作者撤回。
* **已推迟** -- 该FIP正在等待另一个FIP/其他一些与之捆绑的更改。
* **已濒死** -- 该FIP已经实施，现在已经过时，且不再需要替换。


## 优质的FIP需要什么？

每个FIP应包括以下部分：

- 前导码 - RFC 822格式的报头，包含关于FIP的元数据，包括FIP编号、简短的描述性标题（最多44个字符），以及作者的详细信息。
- 简单总结 - “如果你不能简单地解释它，你就不能很好地理解它。”为FIP提供一个简单且通俗易懂的解释。
- 摘要 - 对正在解决的技术问题的简短描述（约200字）。
- 动机 (可选) -  对于想要改进ForTube的FIP来说，动机是至关重要的。它应该清楚地解释：为什么现有规范不足以解决FIP想要解决的问题。没有充分动机的FIP可能会被直接拒绝。
- 规范- 技术规范应该描述新功能的所有语法和语义。
- 理论基础 -  需要通过描述设计动机，以及为何做出特定设计决策的原因来充实规范。它应该描述曾经考虑过的替代设计和相关工作，例如，如何在其他语言中支持该功能。基本原理也可以提供社区达成共识的证据，并对讨论过程中提出的重要异议或关注点进行讨论。
- 测试用例 - 测试用例可以在实施阶段添加，但是在实施之前是必需的。
  
- 放弃版权 - 所有FIP的版权必须属于公众。请参阅底部的放弃版权示例。

## FIP格式和模板

FIP应以[markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)格式进行编写。

图像文件应该包含在该FIP文件夹的`assets` 子目录中，如下所示：
`assets/fip-X` (for fip **X**).  当链接到FIP中的图像时，请使用相对链接，例如`../assets/fip-X/image.png`.


## FIP报头前导码

每个FIP必须以[RFC 822](https://www.ietf.org/rfc/rfc822.txt)格式的报头前导码开头，前面和后面都有三个连字符(`---`)。这个标题也被Jekyll称为[" 前台" ](https://jekyllrb.com/docs/front-matter/)。 报头必须按以下顺序出现。标有 "*"  的报头是可选的，如下所述。所有其他报头都是必需的。



` fip:` <FIP number> （由FIP编辑确定）

` title:` <FIP title>

` author:` <作者姓名和/或用户名，或姓名和电子邮件的列表。详情如下。>

` * discussions-to:` \<指向forum.for.tube的官方讨论主题的url>

` status:` <WIP |提案|批准|实施>

` created:` <date created on>

` * updated:` <comma separated list of dates>

` * requires:` <FIP编号>

` * resolution:` \<指向此FIP决议的url>

允许列入的报头必须用逗号分隔。

需要填写日期的报头需要始终采用ISO 8601（yyyy-mm-dd）格式。



#### `author` 报头

`author` 报头可选择性的列出FIP作者/所有者的姓名、电子邮件地址或用户名。那些喜欢匿名的人可以只使用用户名，也可以使用名字和用户名。作者报头值的格式必须为：

> Random J. User &lt;address@dom.ain&gt;

或者

> Random J. User (@username)

如果包含电子邮件地址或GitHub用户名，以及

> Random J. User

如果没有给出电子邮件地址。

#### `discussions-to` 报头

当FIP处于WIP或“提案”状态时，报头将指向[forum.for.tube](https://forum.for.tube/)论坛中讨论该FIP的地址。

#### `created` 报头

`created`报头记录FIP分配编号的日期。两个报头都应为yyyy-mm-dd格式，例如2001-08-14。


#### `updated` 报头

`updated` 报头记录FIP发生“实质性”更改的日期。此标题仅对草案和活动状态的FIP有效。

#### `requires` 报头

FIP可能具有一个`requires` 报头，指示该FIP所关联的FIP编号。


## 辅助文件

FIP可能包括辅助文件，如图表。这些文件必须命名为FIP-XXXX-Y.ext，其中“XXXX”是FIP编号，“Y”是序列号（从1开始），“ext”被替换为实际的文件扩展名（例如“png”）。



## FIP 编辑

目前FIP编辑为:

` * David (@Master-LY)`

` * Mirai (@Mingliang233)`

## FIP编辑职责

对于每个新的FIP，编辑将执行以下操作：

- 阅读FIP以检查它是否已准备就绪：健全且完整。这些想法必须具有技术意义，即使它们看起来不太可能达到最终状态。
- 标题应准确描述内容。
- 检查FIP的语言（拼写、语法、句子结构等）、标记（Github风格的Markdown）、代码样式
  
如果FIP还没有准备好，编辑会把它发回给作者进行修订，并附上具体的说明。


一旦FIP准备好用于存储库，FIP编辑将：

- 分配一个FIP编号（通常是PR编号，或者，如果作者喜欢，可以是议题编号#如果本存储库的“议题”部分中有关于此FIP的讨论）

- 合并相应的请求

- 向FIP作者发送下一步的消息

FIP编辑监视FIP的更改，并更正看到的任何结构、语法、拼写或标记错误。

编辑们不会评判FIP，只做管理和编辑部分。


## 历史

FIP文档主要来源于SIP Synthetix改进提案文档，在许多地方文本只是简单地复制和修改。有关FIP文件的任何意见都应提交给FIP编辑。

## 版权

通过[CC0](https://creativecommons.org/publicdomain/zero/1.0/)放弃版权和相关权利。




