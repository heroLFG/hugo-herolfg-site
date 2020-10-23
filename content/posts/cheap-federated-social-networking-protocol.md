+++ 
draft = false
date = 2020-10-23T05:23:08-05:00
title = "Cheap Federated Social Networking Protocol"
description = "How to do cheap decentralized social networking."
slug = "cheap-federated-social-networking-protocol" 
tags = ['technology','networking','social','media']
categories = []
externalLink = ""
series = []
+++

# Introduction

Many people want to own their data and the algorithms which are used when engaging with other people on the internet.  I mentioned this idea to a friend and he introduced me to [Mastadon](https://joinmastodon.org/).  I soon learned about [activity pub](https://www.w3.org/TR/activitypub) and the [fediverse](https://en.wikipedia.org/wiki/Fediverse).

I started thinking about how I want to use activity pub.  I could join an existing [Mastadon community](https://joinmastodon.org/communities) or I could host my own server.  I could also look at other open source projects which leverage activity pub.

But I use [hugo](https://gohugo.io/) to build this static site and host it with [github pages](https://pages.github.com/).  It is easy and free for me.  It also uses version control by default.  And I own my data.  What if I could participate in the fediverse in a slightly different way?

# The Protocol

When you use a static website to provide content you can not support POST requests to your site.  All of the requirements in activity pub about POST requests and content type headers are problematic if you want a cheap static site.  And if your networking protocol is restricted to GET requests then you must use a `pull protocol` instead of a push protocol when receiving messages from other people.  This cheaper pull protocol `would not facilitate privacy`.

To receive messages from others, my client application can pull from the `outbox` of all the profiles in my `following` collection.  And to send messages to others, I publish content to my `outbox` for other people to pull from.  It's a very simple protocol which is similar to [RSS](https://en.wikipedia.org/wiki/RSS) but is slightly more complicated in order to facilitate public conversations in a way which allows for better conversation tooling.  The most important difference between RSS and this cheaper version of activity pub is [Audience Targeting](https://www.w3.org/TR/activitystreams-vocabulary/#audienceTargeting) which helps separate the "signal from the noise" and allows for "conversation threads".

One goal I have in this protocol is to allow for a conversation tree to emerge more easily.  I should be able to highlight a word, sentence, or paragraph and reference that highlight in my response to facilitate a mutual understanding of the specific topic each person is trying to have a conversation about.  Conversation tooling can then display the conversation in a tree format.

This cheaper pull based activity pub protocol should be able to work alongside the existing push based activity pub protocol.  My client application can act as a server and try to make POST requests to other people's `inbox` in addition to making the content available in my public `outbox `.  I could also choose to reference an `inbox` hosted by a legit server in my profile to allow people to connect with me.  In this way, the domain for my `inbox` would be different from the domain for my `outbox`.  And my client application could do GET requests to the `inbox` hosted by someone else on my behalf.