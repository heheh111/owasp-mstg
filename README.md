<a href="https://leanpub.com/mobile-security-testing-guide"><img width=180px align="right" style="float: right;" src="Document/Images/mstg-cover-release-small.jpg"></a>


# OWASP Mobile Security Testing Guide [![Twitter Follow](https://img.shields.io/twitter/follow/OWASP_MSTG.svg?style=social&label=Follow)](https://twitter.com/OWASP_MSTG)
[![Creative Commons License](https://i.creativecommons.org/l/by-sa/3.0/88x31.png)](http://creativecommons.org/licenses/by-sa/3.0/ "CC-by-SA 3")
[![OWASP Labs](https://img.shields.io/badge/owasp-lab%20project-f7b73c.svg)](https://www.owasp.org/index.php/Category:OWASP_Project#tab=Project_Inventory)
[![Build Status](https://travis-ci.com/OWASP/owasp-mstg.svg?branch=master)](https://travis-ci.com/OWASP/owasp-mstg)


This is the official GitHub Repository of the OWASP Mobile Security Testing Guide (MSTG). The MSTG is a comprehensive manual for mobile app security testing and reverse engineering. It describes technical processes for verifying the controls listed in the [OWASP Mobile Application Verification Standard (MASVS)](https://github.com/OWASP/owasp-masvs "MASVS").
You can also read the MSTG on [Gitbook](https://mobile-security.gitbook.io/mobile-security-testing-guide/ "MSTG @ Gitbook") or download it as an [e-book](https://leanpub.com/mobile-security-testing-guide-preview "MSTG as an e-book").

## Table-of-Contents

### Introduction

- [Header](Document/0x00-Header.md)
- [Foreword](Document/Foreword.md)
- [Frontispiece](Document/0x02-Frontispiece.md)
- [Introduction to the Mobile Security Testing Guide](Document/0x03-Overview.md)
- [Mobile App Taxonomy](Document/0x04a-Mobile-App-Taxonomy.md)
- [Mobile App Security Testing](Document/0x04b-Mobile-App-Security-Testing.md)

### General Testing Guide

- [Mobile App Authentication Architectures](Document/0x04e-Testing-Authentication-and-Session-Management.md)
- [Testing Network Communication](Document/0x04f-Testing-Network-Communication.md)
- [Cryptography in Mobile Apps](Document/0x04g-Testing-Cryptography.md)
- [Testing Code Quality](Document/0x04h-Testing-Code-Quality.md)
- [Tampering and Reverse Engineering](Document/0x04c-Tampering-and-Reverse-Engineering.md)
- [Testing User Education](Document/0x04i-Testing-user-interaction.md)

### Android Testing Guide

- [Platform Overview](Document/0x05a-Platform-Overview.md)
- [Setting up a Testing Environment for Android Apps](Document/0x05b-Basic-Security_Testing.md)
- [Data Storage on Android](Document/0x05d-Testing-Data-Storage.md)
- [Android Cryptographic APIs](Document/0x05e-Testing-Cryptography.md)
- [Local Authentication on Android](Document/0x05f-Testing-Local-Authentication.md)
- [Android Network APIs](Document/0x05g-Testing-Network-Communication.md)
- [Android Platform APIs](Document/0x05h-Testing-Platform-Interaction.md)
- [Code Quality and Build Settings for Android Apps](Document/0x05i-Testing-Code-Quality-and-Build-Settings.md)
- [Tampering and Reverse Engineering on Android](Document/0x05c-Reverse-Engineering-and-Tampering.md)
- [Android Anti-Reversing Defenses](Document/0x05j-Testing-Resiliency-Against-Reverse-Engineering.md)

### iOS Testing Guide

- [Platform Overview](Document/0x06a-Platform-Overview.md)
- [Setting up a Testing Environment for iOS Apps](Document/0x06b-Basic-Security-Testing.md)
- [Data Storage on iOS](Document/0x06d-Testing-Data-Storage.md)
- [iOS Cryptographic APIs](Document/0x06e-Testing-Cryptography.md)
- [Local Authentication on iOS](Document/0x06f-Testing-Local-Authentication.md)
- [iOS Network APIs](Document/0x06g-Testing-Network-Communication.md)
- [iOS Platform APIs](Document/0x06h-Testing-Platform-Interaction.md)
- [Code Quality and Build Settings for iOS Apps](Document/0x06i-Testing-Code-Quality-and-Build-Settings.md)
- [Tampering and Reverse Engineering on iOS](Document/0x06c-Reverse-Engineering-and-Tampering.md)
- [iOS Anti-Reversing Defenses](Document/0x06j-Testing-Resiliency-Against-Reverse-Engineering.md)

### Appendix

- [Testing Tools](Document/0x08-Testing-Tools.md)
- [Suggested Reading](Document/0x09-Suggested-Reading.md)

## Reading the Mobile Security Testing Guide

The release 1.0 of the MSTG was published in June 2018. You can get intermediate builds in multiple formats.

1. Read it on [Gitbook](https://mobile-security.gitbook.io/mobile-security-testing-guide/ "Gitbook"). The book is automatically synchronized with the main repo.

2. Check the [releases](https://github.com/OWASP/owasp-mstg/releases "Our releases"). Here you can find a PDF, an archive containing the sources and a DocX document for any given tagged version. Please note that the documents are generated automatically per tag.

3. Get the [e-book](https://leanpub.com/mobile-security-testing-guide-preview "MSTG as an e-book"). The book is available for free, but you can choose to purchase it at a price of your choosing if you wish to support our project. All funds raised through sales of the e-book go directly into the project budget and will be used to fund production of future releases.

3. Clone the repository and run the [document generator](https://github.com/OWASP/owasp-mstg/blob/master/Tools/generate_document.sh "The document generator") (requires [pandoc](http://pandoc.org "Pandoc")). This produces docx and HTML files in the "Generated" subdirectory.

```shell
$ git clone https://github.com/OWASP/owasp-mstg/
$ cd owasp-mstg/Tools/
$ ./generate_document.sh
```

4. Clone the repository and run the [gitbook generator](https://github.com/OWASP/owasp-mstg/blob/master/Tools/gitbookepubandpdf.sh "Gitbook based"). This produces PDF, Epub and Mobi files in the "Generated" subdirectory.

```shell
$ git clone https://github.com/OWASP/owasp-mstg/
$ cd owasp-mstg/Tools/
$ ./gitbookandpdf.sh
```

You can also use the [document index](https://rawgit.com/OWASP/owasp-mstg/master/Generated/OWASP-MSTG-Table-of-Contents.html "TOC") to navigate the master branch of the MSTG.

## Contributions, feature requests and feedback

**We are searching for additional authors, reviewers and editors.** The best way to get started is to browse the [existing content](https://mobile-security.gitbook.io/mobile-security-testing-guide/ "existing content"). Also, check the [issues](https://github.com/OWASP/owasp-mstg/issues "our issues section") and the [project page](https://github.com/OWASP/owasp-mstg/projects/2 "The MSTG Project") for a list of open tasks.

Drop a us line on the [Slack channel](https://owasp.slack.com/messages/project-mobile_omtg/details/ "Come to Slack!") before you start working on a topic. This helps us to keep track of what everyone is doing and prevent conflicts. You can create a Slack account here:

[https://owasp.slack.com/](https://join.slack.com/t/owasp/shared_invite/enQtNDI5MzgxMDQ2MTAwLTEyNzIzYWQ2NDZiMGIwNmJhYzYxZDJiNTM0ZmZiZmJlY2EwZmMwYjAyNmJjNzQxNzMyMWY4OTk3ZTQ0MzFhMDY)

Before you start contributing, please read our brief [style guide](https://github.com/OWASP/owasp-mstg/blob/master/style_guide.md "Style Guide") which contains a few basic writing rules.

Please note that the MSTG focuses primarely on the native apps. These are apps built with Java or Kotlin using the Android SDK for Android or built with Swift or Objective-C using the Apple SDKs for iOS. Nativescript/React-native/Xamarin/Cordova/... apps are not within the focus of the MSTG. However, some key-controls, such as pinning, have been explained already for some of these platforms.

If there's something you really want to see in the guide, or you want to suggest an improvement, create an issue [issue](https://github.com/OWASP/owasp-mstg/issues "Issue") or ping us on [Slack](https://owasp.slack.com/messages/project-mobile_omtg/details/ "Come to our Slack!").
If the issue is accepted, we will schedule it into one of our [milestones](https://github.com/OWASP/owasp-mstg/milestones "Milestones").

### Translating
Our current goal is to publish one minor release every 6 months. Next, we will often create patch updates in order to provide intermediary updates in PDF and DocX format. Releases that have been tagged can then be translated into preferred languages.
(Note we use semantic versioning: major.minor.patch)


### Contributing

- Fork it ( https://github.com/[my-github-username]/owasp-mstg/ )
- Create your feature branch (git checkout -b my-new-feature)
- Commit your changes (git commit -am 'Add some feature')
- Push to the branch (git push origin my-new-feature)
- Create a new Pull Request
- The project leaders will QA and give feedback before it's merged.

## Authoring Credit

Contributors are added to the acknowledgements table based on their contributions logged by GitHub. The list of names is sorted by the number of lines added. Authors are categorized as follows:

- Project Leader / Author: Manage development of the guide continuously and write a large amount of content.
- Co-Author: Consistently contribute quality content, [at least 2,000 additions logged](https://github.com/OWASP/owasp-mstg/graphs/contributors "Co-author").
- Top Contributor: Consistently contribute quality content, [at least 500 additions logged](https://github.com/OWASP/owasp-mstg/graphs/contributors "Top Contributor").
- Contributor: Any form of contribution, [at least 50 additions logged](https://github.com/OWASP/owasp-mstg/graphs/contributors "Contributor").
- Mini-contributor: Everything below 50 additions, e.g. committing a single word or sentence.
- Reviewer: People that haven't submitted their own pull requests, but have created issues or given useful feedback in other ways.

Please ping us or create a pull request if you are missing from the table or in the wrong column (note that we update the table frequently, but not in realtime).

If you are willing to write a large portion of the guide and help consistently drive the project forward, you can join as an author. Be aware that you'll be expected to invest lots of time over several months. Contact Sven Schleier (Slack: *sushi2k*) or Jeroen Willemsen (Slack: *jeroenwillemsen*) for more information.

## Crackmes
In the Crackmes folder, you can find a set of mobile apps to hack. Are you able to find the secrets? For more details: check the [README.md](https://github.com/OWASP/owasp-mstg/blob/master/Crackmes/README.md "Crackmes readme") at the [Crackmes folder](https://github.com/OWASP/owasp-mstg/blob/master/Crackmes "Crackmes folder").
