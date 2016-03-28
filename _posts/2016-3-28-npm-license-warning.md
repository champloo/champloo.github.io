---
layout: post
title: npm license warning
---

Got a bit sick of seeing the license warning every time I ran npm. You know the one that says _'No license field'_ or _'license should be a valid SPDX license expression'_.

I previously removed the the license field from package.json since I am working on a personal project that is not open source, so the SPDX licenses do not apply. This causes the _'No license field'_ warning. I then tried changing the license to _'private'_ and other random strings but that spits out the second warning.

It turns out setting the license to __UNLICENSED__ is the correct way to deal with this according to https://github.com/npm/npm/issues/8291. Warnings be gone!
