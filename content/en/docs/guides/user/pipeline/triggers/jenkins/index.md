---
title: "Triggering pipelines with Jenkins"
linkTitle: "Triggering pipelines with Jenkins"
weight: 
description: >
  This guide explains how add a [Jenkins](https://jenkins.io/) trigger to your pipeline.
---


This guide explains how add a [Jenkins](https://jenkins.io/){:target="\_blank"}
trigger to your pipeline.

## Prerequisites

*   [Set up Jenkins](/setup/ci/jenkins/) as a continuous integration system in
    your Spinnaker deployment

## Adding a Jenkins trigger

1.  [Create a pipeline](/docs/v1/guides/user/pipeline/managing-pipelines/#create-a-pipeline).
1.  In the **Configuration** stage of your new pipeline,
    [add a trigger](/docs/v1/guides/user/pipeline/managing-pipelines/#add-a-trigger).
1.  Select **Jenkins** from the **Type** menu, which brings up the following
    screen:
    ![](add-trigger.png)
1.  Select a Jenkins master from the **Master** drop-down menu, and a job from
    the **Job** drop-down. These will be automatically populated if you have set
    up Jenkins correctly.
1.  Add a property file, if desired. See the [property
    files](/docs/v1/guides/user/pipeline/expressions/#property-files) section of the
    Pipeline Expression Guide for more information about how to specify and use
    property files.