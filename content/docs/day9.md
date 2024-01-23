+++
title = 'Day 9: Headless CMS Rabbit Hole'
date = 2024-01-23T22:36:48+08:00
draft = false
+++

I've spent the past few days looking for a headless CMS to include in the [LaunchYourList.com](https://www.launchyourlist.com) template stack. To be honest, this would have been an easier task if I were just building this template for myself! However, since I plan to share it with non-tech friends who will have access to the code itself, I'm trying to make it as painless as possible to setup and use.

Here are the options I have considered so far and my thoughts on each:

1. [Strapi](https://strapi.io/) - It's suitable for me as a developer but might be challenging for non-tech users.

2. [PayloadCMS](https://payloadcms.com/) - It follows a code-first philosophy, which is okay for me as a developer, but it may also be challenging.

3. [Pocketbase](https://pocketbase.io/) with [Pockethost](https://pockethost.io/) - This is my top choice so far. It offers a painless experience and has a great developer experience (DX). Pocketbase's admin dashboard looks fantastic, and that's a significant factor in why I'm leaning towards this option.

4. [Firebase](https://firebase.google.com/) with [FireCMS](https://firecms.co/) / [Rowy](https://www.rowy.io/) - I really wanted to choose this one since I've been using Firebase for years, but I don't like the user interface/user experience (UI/UX) of its CMS offerings. Additionally, there may be a vendor lock-in to consider, but this is really a non-issue for a small product at this point.

5. **The "IDEAL" CMS FOR ME** - Something that combines the developer experience (DX), UI, and UX of Pocketbase + Pockethost but uses Firebase as the database and file storage.
