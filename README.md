<div align="center">
<img src="Heading.svg" width="360">
<br>
</div>

# Project GuOJ 🔭🕊️

![contributors](https://img.shields.io/github/contributors/guoj-dev/GuOJ)
![license](https://img.shields.io/github/license/guoj-dev/GuOJ)
![forks](https://img.shields.io/github/forks/guoj-dev/GuOJ)
![stars](https://img.shields.io/github/stars/guoj-dev/GuOJ)
![issues](https://img.shields.io/github/issues/guoj-dev/GuOJ)
![issues-pr](https://img.shields.io/github/issues-pr/guoj-dev/GuOJ)

The Heading and Logo of this project is now a Noto Emoji re-creation. Please note that it's original licensed under Apache-2.0.

---

> We are the people who code, who dream, who live.

English | [简体中文](https://github.com/guoj-dev/GuOJ/blob/master/README_zh.md)

Project GuOJ is an open source project which implements a modern online judge system contains features like online code judging, holding contests, organizations and lots of new features. It aims at develop a platform for GuOJ which is a community provides an excellent experience for any level programmers, computer science lovers. We work for people in Olympic Informatics, Collegiate Programming Contest, and generic algorithms.

## Our Purpose 🛠️💭

Nowadays, we got a bunch of online coding communities all over the world. Our target is making this project and the community a better experience, without any compromises.

The judge system is the main part of an online judge system. Judge systems have no common standards but primitive POSIX file standard or some specific standard like `testlib` which is not unified. Our vision is defining a unified judge standard can be used for any programming language and contains modern features. It has to be customizable and flexible. Compatibility is important, but we don't want to make any compromises. The final target is you can just write a simple config file or configure it by a web interface to complete a migration of a common algorithm. And it will be easy to convert it to a unified standard problem with detailed guidance.

The problem exhibition is also an important part of the online judge system. We decided to make a modern web interface. All the problems will showed in XSS-free markdown documents. This is the solution used by current online judge systems. However, we still have issues on showing lots of contents like raw HTML or PDF which is complicated if we use pure markdown. To solve this problem, we will make the problem page is configurable and compatible with raw HTML, raw PDF and other types maybe. The only limit is we will make sure all the content is XSS-free and safe because we have plans for UGC (User Generated Content).

The contest system is an important part for competitive programming. The whole system is still open to discussion. But We'd like to share our plans now, to find lacks and potential improvements. The contest system is meant to be customizable and flexible. It is designed to fit most forms of programming contests, users can specify the rules, the features, the way it judges. To simplify this, we will make preset contest rules to help you kickstart your contest fast and painless, and you can simply make your own rules by editing existing rules or read our guides and documents. We want to make it painless on holding and enjoying your contest. There will be also addtion features or tools to help you enrich your contest. We will provide tools helping you get your data in your contest for some specific purposes like rolling prizes. There will be a series of community tools for contesters and holders like annoncements, discussions. They will be pretty customizable to make sure your contest is will prepared and have an excellent experience.

The community part is the hugest part besides the online judge system. We think this is the main difference and the most revolutionary part of the project. The first part is a forum system, We have topic based forums for everyone, and we hope everyone can have the best experience in discuessing everything related to your favourite topics. In addition, we will provide problem, contest, even problemset related tags for discussing problems, contests etc. To avoid it cannot be seen, the discussion with certain tags will be shown in specific pages and can be seen by everyone visit this page. Also, we will provide a Q&A feature. It should have Quora-like experience. The second part is a micro blogging system with modern timeline support, we will provide a promising experience like trending social media platforms, and the open source project mastodon. We maybe add a support to the protocol mastodon is using in the future, maybe a mobile platform support too. We want to make this be your last tech-related social media platforms, deliver you informations by a open community. Also, we maybe provide a IM platform powered by another open source project `rocket.chat`. But it's not our main goal now, and I'm afraid we don't have enough resources on it. It depends on the future of this project.

## Our advantages ⚡🌌

The whole project is delivering by an open source community. The effort we put in, the changes we make is open and transparent, can be used by latecomers. We are working on modern web technology stack. Our frontend is using Vue 2.0 and Vuetify. It's a blazing fast web framework and contains amazing material design components. Our backend is using Nest.JS, Prisma and GraphQL as API endpoints. We don't have plan for global extensions or all-in-one extension standard for every part of this project now, but we may put some effort on make some specific part of the project is extension friendly, and there will be a friendly document for API and the architecture, which would help you to get the main idea of the project and make changes on our code as fast as you can.

We want to create a place that nothing else could like this. This could only be made by us, the community. We believe the community driven community is the best solution. Our project depends on our community.

## Project Roadmap 🚥🚧

We're current on the early stage of this project. But we think a clear roadmap is necessary for a healthy life cycle. Now we will list our project on the road or in progress. Feel free to give us your advice.

### Project MCV - The Judge Client ⚛️🔨

MCV, or `Minimum Container Vehicle` is the minimum unit of the judge system. It contains a container environment for compiling and running the judge session. Like many projects have the same feature, it is based on `cgroup` and `ptrace`, uses `OCI runtime` as the container environment. Previous similar projects has proved and implement the secure sandbox, base on this, we want to make the standardize the protocol and make it can carry out different types of tasks. We want to specific a task definition standard and a judge session communication protocol.

### Judge@Home - The Distributed Judge Unit Manager 🏠🤝

`Judge@Home`, is a distributed judge unit manager. The judge server need a lot of resources. We define a "judge client" is a `Judge@Home` instance with several MCV judge client in the main server. User can register a judge account and connect their self-host `Judge@Home` instance to the server. You can select the judge strategy, to only receive your private judge session for better performance or applying special configuration, or register as a global judge instance. If you are working as a global instance, you must be certified to join the default judge queue, or you will be a selectable judge instance for all users. We want to make sure the performance and validity of the global judge sessions, so we need to put more efforts on this. So this project will begin later and must be tested to be put in production.

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

This project is licensed under GNU Affero General Public License. The artworks are licensed under CC BY-NC-SA 4.0 License.

![CC BY-NC-SA 4.0 Badge](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)
