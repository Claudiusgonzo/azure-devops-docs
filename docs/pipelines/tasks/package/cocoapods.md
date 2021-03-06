---
title: CocoaPods task
ms.custom: seodec18
description: Learn all about how you can use CocoaPods packages when you are building code in Azure Pipelines or Team Foundation Server (TFS).
ms.topic: reference
ms.assetid: D690542B-9A13-4836-8C1E-D715AE6CB7D6
ms.author: vijayma
author: vijayma
ms.date: 08/10/2016
monikerRange: '>= tfs-2015'
---

# CocoaPods task

[!INCLUDE [temp](../../includes/version-tfs-2015-rtm.md)]

Use this task to run CocoaPods [pod install](https://guides.cocoapods.org/using/pod-install-vs-update.html).

[CocoaPods](https://cocoapods.org/) is the dependency manager for Swift and Objective-C Cocoa projects. This task optionally runs `pod repo update` and then runs `pod install`.

## Demands

None

::: moniker range="> tfs-2018"

## YAML snippet

[!INCLUDE [temp](../includes/yaml/CocoaPodsV0.md)]

::: moniker-end

## Arguments

<table><thead><tr><th>Argument</th><th>Description</th></tr></thead>
<tr><td>Working directory</td><td>(Optional) Specify the working directory in which to execute this task. If left empty, the repository directory will be used.</td></tr>
<tr><td>Force repo update</td><td>(Required) Selecting this option will force running &#39;pod repo update&#39; before install.</td></tr>
<tr><td>Project directory</td><td>(Optional) Optionally specify the path to the root of the project directory. If left empty, the project specified in the Podfile will be used. If no project is specified, then a search for an Xcode project will be made. If more than one Xcode project is found, an error will occur.</td></tr>


<tr>
<th style="text-align: center" colspan="2"><a href="~/pipelines/process/tasks.md#controloptions" data-raw-source="[Control options](../../process/tasks.md#controloptions)">Control options</a></th>
</tr>

</table>

## Open source

This task is open source [on GitHub](https://github.com/Microsoft/azure-pipelines-tasks). Feedback and contributions are welcome.

## Q & A

<!-- BEGINSECTION class="md-qanda" -->

[!INCLUDE [temp](../../includes/qa-definition-common-all-platforms.md)]

[!INCLUDE [temp](../../includes/qa-agents.md)]

::: moniker range="< azure-devops"

[!INCLUDE [temp](../../includes/qa-versions.md)]

::: moniker-end

<!-- ENDSECTION -->
