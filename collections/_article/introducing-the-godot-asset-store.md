---
title: "Introducing the Godot Asset Store"
excerpt: "We've been working on replacing the Asset Library with something built for the present and future. Here's what's coming."
categories: ["news"]
author: Emi
image: /storage/blog/covers/godot-asset-store.jpg
date: 2026-05-19 18:30:00
---

After many years of having the [Asset Library](https://godotengine.org/asset-library/asset) as the only "official" place to publish assets, we attempted to modernize it and started building upon it to address the major pain points and user requests. Unfortunately, while doing that, we noticed how challenging dealing with that code was. From the user accounts to the way templates and information are displayed, the current Asset Library code is inflexible and fragile.

You already know that we have been using a shared account system across all of our online platforms. This means you can use your Godot account to chat on our [developer chat](https://chat.godotengine.org/), participate on [the forum](https://forum.godotengine.org/), vote for [showreel candidates](https://showreel.godotengine.org/), and donate to the [development fund](https://fund.godotengine.org/). Unfortunately, the Asset Library was set up with a separate account system, so you have to maintain yet another Godot account specifically for it. That account system has been plagued with many issues, from spam to password reset emails not arriving, that required a lot of manual work to operate. This wasn't a problem in the past, but with [more users using Godot](https://godotengine.org/article/godot-growth-stats-2026/), we need to spend an increasing amount of resources here.

Over the past few years, we managed to squeeze some improvements in, but most of them were cosmetic. As soon as we got into editing the code, we noticed how brittle everything was, and if we wanted to make drastic changes, we would still need to address major foundational issues while also maintaining compatibility with older versions of the Godot editor. Instead, we decided to start from scratch with the present and future needs in mind, and create the new [Godot Asset Store](https://store.godotengine.org/).

![A screenshot of the Godot Asset Store](/storage/blog/asset-store/godot-asset-store-screenshot.webp)

## The [Godot Asset Store](https://store.godotengine.org/)

We initially didn't have plans to run an asset store operated by the Foundation. With most projects outside of the Godot Engine itself, we try to foster an ecosystem that provides solutions Godot developers need, and we expected someone to make and run an asset store with Godot in mind. There were also existing stores that people use (like [itch](https://itch.io/search?q=godot)), so we assumed the community would centralize around the one that worked best for them.

Unfortunately, when a few unofficial store pages started to show up hosting paid assets, they were purposefully misleading users into thinking the Godot Foundation was running them. We even started receiving regular support emails from users trying to get refunds on assets that were never delivered or payments that never arrived. These stores were also hosting paid versions of free assets (such as [Kenney's](https://www.kenney.nl/)) with unclear information about ownership or transparency.

Thankfully, these stores were never popular enough to be a serious issue, and many have already closed since then, but it's not a great situation to leave for each user to deal with.


![A screenshot of the Godot Asset Store](/storage/blog/asset-store/godot-asset-store-screenshot-2.webp)

## Replacing the Asset Library

Since it was clear that the Asset Library was going to be hard to improve, and there was real demand for a store, we didn't think it was efficient to run two different platforms at the same time, so the project to replace the old Asset Library with the new Asset Store was kickstarted.

We will still need to keep the Asset Library running for a while since many older versions of the engine will still need it, but the ultimate goal is to deprecate it and leave it as a read-only repository.

We considered moving the assets from the library to the new store, but it wasn't feasible. We would first need everyone to create a new account and link them together (which would require changes to the old account system), then get permission from each asset author to republish on their behalf, and since the current Asset Library doesn't actually host any of the assets it distributes, we would need to re-upload all of them to the new hosting solution. There are also many differences in how assets are presented that would make the migration incomplete, and many of them have been abandoned or are no longer supported, so it would just create a lot of irrelevant entries in the new store.

The new Godot Asset Store is still under development, but it already has far more features than the Asset Library: user reviews, multiple download versions per asset, tags, analytics, changelogs, and many more coming in the future (check out the [roadmap](https://store.godotengine.org/roadmap/)). Once this transition is finished, we will be able to make bigger improvements in both the online store and the tab inside the Godot Engine editor.

## Future

Being able to sell and buy assets is one of the most anticipated features of the Asset Store, but we want to make sure the transition away from the Asset Library is fully complete before enabling this. Buying and selling assets will give us a bit of extra funding to hopefully cover the costs of operating the store, but profit is not the Godot Foundation's priority for this project. You might notice that progress on the Asset Store is not fast, because we are still going to be prioritizing the Godot Engine above any other project. So while we want to foster a space for people who up until now haven't been very engaged with the Godot community (primarily non-programmers), we also want it to be a space that's safe, functional, and up to the quality standards you'd expect from an asset store.

We also want to make it easier for users to donate to free plugins. Many popular projects (like [Phantom Camera](https://store.godotengine.org/asset/ramokz/phantom-camera/), [Dialogue Manager](https://store.godotengine.org/asset/nathanhoad/dialogue-manager/), and [GodotSteam](https://store.godotengine.org/asset/godotsteam/godotsteam-gdextension/)) have been at the core of many existing projects, but this isn't translating well into donations. We hope that with the new Asset Store, donating to these plugins will become more common and give them the support they deserve to keep their assets free and open source for everyone.

The Godot Foundation will use the Asset Store to publish official plugins and extensions we are working on that we don't believe should be part of the core experience, but we have no plans to sell any assets ourselves. As with Godot, everything we publish will be free and open source.

This is just the beginning, and we really value your feedback and input. We want to hear your thoughts, and we will keep making changes and adjusting to make sure the [Godot Asset Store](https://store.godotengine.org/) is what you need and what you expect from it. So feel free create an [issue on our tracker](https://github.com/godotengine/godot-asset-store-tracker/issues), [open a discussion](https://github.com/godotengine/godot-asset-store-tracker/discussions), or get in touch via email at [contact@godot.foundation](mailto:contact@godot.foundation). 

We'll keep you all posted regarding the improvements of the store so expect to hear from us soon.