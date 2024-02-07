Here's a proofread version of your text:

+++
title = 'Day 19-25: Got Sick, Downshift, MiniSearch, useTransition'
date = 2024-02-07T22:59:37+08:00
draft = false
+++

I forgot to publish a blog on Friday (Feb 2) and then got sick when I arrived in Manila, so I missed several days of blogging.

Anyway, while I was out, I learned a lot of new things while implementing a basic search for [LaunchYourList](https://launchyourlist.com).

Here's a summary of it:

- Use [Downshift](https://www.downshift-js.com/) for your search bar auto-completes & suggestions. I thought using it was overkill at first until I realized that we take a lot of small things for granted when it comes to the standard search UX that you and I, as users, frequently experience.
- Use [MiniSearch](https://lucaong.github.io/minisearch/) if you need lightweight search.
- I just found out there's a hook called [useTransition](https://react.dev/reference/react/useTransition). Not sure yet as to what other use cases it might have, but I'm using it when updating the current search params of the page URL.
- I learned how to implement a search that has a client-side search bar with a server-side component for the results list. Check it out [here](https://x.com/ryantotweets/status/1622632894278533130?s=20)!
