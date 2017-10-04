---
layout: post
title: test title2
published: false
---
How to make your own opensource java/scala library with sbt and publish it to jitpack.io

**1) Create empty sbt project**
If you using mac or linux the simplest way - creating scripts with followings content:

    #!/bin/sh
    mkdir -p src/{main,test}/{java,resources,scala}
    mkdir lib project target

    # create an initial build.sbt file
    echo 'name := "MyProject"
    version := "1.0"
    scalaVersion := "2.12.2"' > build.sbt

