+++
title = 'Day 16: "flatMap" in RxSwift'
date = 2024-01-30T23:14:58+08:00
draft = false
+++

I've been using this operator for a long time but kinda forgot it because I'm pivoting to web, but today there was a necessity to recall it in one of the enterprise apps my team is working on.

Using "flatMap" is pretty straightforward. It allows you to connect observables in a sequentially chained manner rather than a nested one, resulting into a single observable to be subscribed to.
