---
layout: post
title:  "Revisiting AR"
date:   2022-07-29 10:00:00 -0700
categories: Augmented Reality
tags: AR, spiking
---

it’s been quite a while since i posted, but as i start on the journey of learning and eventually masting ARKit, i decided that i would document it (just as i have recommended others). **fingers-crossed** i intent to post regularly, sharing my progress.

Revisiting? yes. this is definitely not my first endeavor into building Augmented Reality applications. Back in 2011, we (my partner in code & friend Kaza) were attempting to build AR games way before ARKit was announced or even possible. The current iPhone at the time was the iPhone 4 which was at the time one of the most powerful handheld computer, but still was underpowered by modern standards. At the time Qualcomm offered the best libraries to support AR on iOS, but it was still very limited. The biggest missing piece was ARKit. Without a first party API for determining the physical position of the device in the real world, developers only option was to leverage the existing capabilities of Core Motion and Core Location frameworks.

Enter “Sensor Fusion”. This was my attempt to collect all the relative sensor data from the aforementioned frameworks to produce an estimation of the device position was. This was quite a task and kinda worked. The problem was that it was very slow, so after some optimizations, separating the data processing into a background thread and propagating the position information to the main/UI thread on a schedule, we had something that met our needs. After working on a couple different AR game concepts we arrived at the agreement that the hardware and supporting software just weren’t ready for the immersive experiences we were trying to build. We even spent some time trying build our concepts in Unity3D, but the tracking was easy to break ruin the the entire experience. Eventually we shelved those projects and never really returned to them
I have barely touched any AR since then, aside from playing with some of the apps and games that have been released over the last few years. When ARKit was announced Kaza and I laughed about how great it’d have been if we had it back when then. This is a recurring theme, we build something years too early and then have moved on by the time tech or user interest has caught up. I actually still haven’t cracked open an ARKit project so I’m really interested in seeing how this goes.