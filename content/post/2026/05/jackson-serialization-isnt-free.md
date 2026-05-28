---
title: "Jackson Serialization Isnt Free"
date: 2026-05-28T10:43:49-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: false
---

I've been doing some upgrades at work, effectively Spring Boot 3 - 4 which includes some Jackson serialization changes.  Lots of changes which make it far less convenient but it is what it is.  So I was googling on some errors that I was getting and while doing so I ran across [this article](https://levelup.gitconnected.com/the-hidden-cost-of-jackson-serialization-425612a4ac06) which goes over someones experience optimizing their AWS bill effectively.  Their stated savings - $4,500 a month!!!  Just from optimizing serialization.  Go give it a read, you'll thank the author, I promise.

Let's pay Big Tech less money!!