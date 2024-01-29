+++
title = 'Day 15: Obscure Iframe and Next.js SSR Bug'
date = 2024-01-29T22:59:29+08:00
draft = false
+++

For some reason adding `<link rel="stylesheet" href="styles.css">` on your HTML's `<head>` and then load it in an iframe owned by a SSR'd page, it will create an odd `styles.css` file that contains the rest of the code for the HTML.

This also causes the the SSR page to have `styles.css` in it's query if it's a dynamic route.
