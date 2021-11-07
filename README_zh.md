# Project GuOJ 🔭🕊️

![](https://img.shields.io/github/contributors/guoj-dev/GuOJ)
![](https://img.shields.io/github/license/guoj-dev/GuOJ)
![](https://img.shields.io/github/forks/guoj-dev/GuOJ)
![](https://img.shields.io/github/stars/guoj-dev/GuOJ)
![](https://img.shields.io/github/issues/guoj-dev/GuOJ)
![](https://img.shields.io/github/issues-pr/guoj-dev/GuOJ)

> We are the people who code, who dream, who live.

Project GuOJ是一个实现了一个包括在线代码评测、比赛举办、团队功能以及一系列新功能的在线评测系统的开源项目。它的目标是为GuOJ这个为任何水平的计算机爱好者以及程序员提供服务的社区开发一个平台。我们服务信息学奥林匹克竞赛、大学生程序设计竞赛以及常规算法竞赛。

## 我们的愿景 - Our Purpose 🛠️💭

我们能在当下的互联网上寻找到许许多多的在线编程社区。但我们的目的是让这个项目以及这个社区拥有一个从不妥协的、更好的体验。

评测系统是一个在线评测系统的一个主要部分。当下的评测系统没有一个统一通用的标准，一般采用POSIX文件标准或一些特定标准如```testlib```，本身无法做到统一。我们希望定义一个统一而且通用的评测系统可以适用于任何编程语言，包含现代化的特性。我们希望做到更加可定制，并且更加灵活。兼容性对我们而言无疑是重要的，但我们不会因此做出妥协。最终的目标是您仅仅需要写一些简单的配置文件甚至是用一个简单的Web界面就能完成对一个算法问题的移植，而且您可以快捷地将它转换为一个更加通用标准下的算法问题，这之中一切过程都会有详细的文档与指导。

题目的展示功能也是一个在线评测系统的重要部分。我们会开发一个现代的Web界面，而所有的题目将会被展示为一系列经过XSS过滤的Markdown文档。这同样是其他现有在线评测系统中比较主流的解决方案。但是这种方案对于一些原生HTML文件以及PDF文件格式的题目并不友好。为了解决这个问题，我们将会留给题目展示页面一些配置的空间，并允许一定程度上的原生HTML文件、PDF文件以及一些其他的文件格式。对此唯一的限制是我们会限制内容的引用以及对内容进行XSS过滤避免开放给用户编辑与创作中潜在的安全性问题。

比赛功能对于算法竞赛以及程序设计竞赛用途而言是一个重要的组成部分。这一部分系统仍需商榷，不过我们仍然愿意与您分享我们目前的计划，从而找出其中的问题以及潜在的提升空间。比赛系统同样需要可定制性与灵活性。它将会被设计成适应各种类型的程序设计竞赛。用户可以自定义规则、一些特殊特性、甚至是评测方式。为了简化这一切，我们会预置一些比赛规则帮助你快速配置好你的比赛，并且你还能简单地定制出你的比赛规则，只需要通过修改已有的比赛规则或是阅读我们的指南和文档。我们希望解决在您举办并享受比赛时出现的痛点。不仅如此，项目还会包含更多附加特性以及工具帮助您丰富您的比赛，例如赛后抽奖工具。还有一些社区类功能比如赛时公告板和赛时讨论区。一切都将有可观的可定制性来确保比赛可以被配置得适应需求，提供一个精彩绝伦的体验。

社区功能是整个系统中在线评测系统之外最大的一个部分。我们认为这会是我们与其他已有在线评测系统最大的差异点。第一个部分是论坛系统。我们将会采用以话题分开的多版块论坛，提供给全体用户。我们希望任何人在讨论任何你感兴趣的话题的同时，拥有最佳的体验。除此之外，我们还会提供题目、比赛，甚至是题库的标签，与这些功能本身紧密集成来满足您讨论的需求。为了防止您的话题不能被发现，这些讨论都会在对应的页面中被展示出来。未来我们还会提供一个提问功能，它将具有与Quora、知乎等问答社区类似的体验。第二个部分是一个“微博”（更像是Micro Blogging或是Twitter，而非商业产品‘Weibo’。）功能，同时具有一个现代化的时间线功能。我们希望提供一个可以与现代主流社交媒体平台以及开源社交媒体软件Mastodin相匹敌的匹敌。同时，我们还可能支持Mastodon等开源去中心化社交媒体所使用的协议，甚至可能支持移动平台应用。我们希望这能够成为你的最后一个关于技术的社交媒体平台，让一个开放的社区为你带来你所需要的信息。不仅如此，我们未来甚至可能会提供一个基于开源IM平台“rocket.chat”的IM平台，虽然这目前并不是我们的主要目标，同时我们也可能不会拥有足够的资源来实现这一愿景，这取决于未来我们的项目究竟会进行到哪一步。

## 我们的优势 - Our advantages ⚡🌌

这个项目由一个开源软件社区打造。我们的投入以及做出的改变是完全开放且透明的，也能被后继者利用。我们的工作基于现代Web技术栈。我们的前端正在使用Vue 2.0和Vuetify。这是一个高效的Web框架而且包含了许多基于Material Design的组件。我们的后端基于Nest.JS、Prisma，使用GraphQL作为API Endpoint。我们对于为这个项目的每一个部分都定义一个全局插件或者统一的插件标准没有计划，但我们可能会做一些微小的工作使得某些特定的部分是可扩展的，并且对于接口与架构我们将会提供友好的文档，这将会对您更好地理解本项目并且快速对本项目做出您独特的修改有着显著的帮助。

我们想要创造一个无可比拟的社区，而这一切只能由各位，也就是我们的社区成员来达成。我们相信由社区驱动的社区是最佳方案。而我们的项目也依赖于我们的社区。

## 项目规划 - Project Roadmap 🚥🚧

我们目前仍然处于整个项目的早期阶段，但我们认为一个详细的项目规划对于一个健康的项目生命周期是必要的。我们将会列出我们的项目进展以及预期成果。请尽情向我们提出您关于这个项目的建议。

### Project MCV - 评测机客户端 ⚛️🔨

MCV，全称```Minimum Container Vehicle```，是整个评测系统的最小单元。本项目包含一个基于容器的评测环境用于编译及运行评测任务。就像其他许多提供相似功能的项目，这个项目基于```cgroup```和```ptrace```，并使用```OCI runtime```作为本项目的容器环境。以前的类似项目已经证明且实现了类似的安全沙盒环境。基于这一切，我们希望标准化所使用的协议并使本系统可以承担不同类型的评测任务。同时，我们希望定义一个评测任务定义规范以及评测任务通讯标准。

### Judge@Home - 分布式评测单元管理系统 🏠🤝

```Judge@Home```, is a distributed judge unit manager. The judge server need a lot of resources. We define a "judge client" is a ```Judge@Home``` instance with several MCV judge client in the main server. User can register a judge account and connect their self-host ```Judge@Home``` instance to the server. You can select the judge strategy, to only receive your private judge session for better performance or applying special configuration, or register as a global judge instance. If you are working as a global instance, you must be certified to join the default judge queue, or you will be a selectable judge instance for all users. We want to make sure the performance and validity of the global judge sessions, so we need to put more efforts on this. So this project will begin later and must be tested to be put in production.

### Project N - The Judge Network Center 🌐🗺️

**_🚧🚧This part is currently WIP, will be finished later, needs more time and suggestions.🚧🚧_**

### Project Meloetta - The Website System 🎨🖌️

**_🚧🚧This part is currently WIP, will be finished later, needs more time and suggestions.🚧🚧_**

### Project Shikieiki - The Universal Judge Library 🔎⚒️

**_🚧🚧This part is currently WIP, will be finished later, needs more time and suggestions.🚧🚧_**

### Project Hieda - The Problem Production Helper ✒️📋

**_🚧🚧This part is currently WIP, will be finished later, needs more time and suggestions.🚧🚧_**

### Project Okina - The Multiplatform Community Client 💻📱

**_🚧🚧This part is currently WIP, will be finished later, needs more time and suggestions.🚧🚧_**

## Code of Conduct 🤝

**_🚧🚧This part is currently WIP, will be finished later.🚧🚧_**

## How to contribute ✊

**_🚧🚧This part is currently WIP, will be finished later.🚧🚧_**

## License 📋

This project is licensed under GNU Affero General Public License. The artworks are licensed unser CC BY-NC-SA 4.0 License.

![CC BY-NC-SA 4.0 Badge](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)
