+++
title = 'Day 30: Dynamic Tailwind CSS Colors in NextJS'
date = 2024-03-23T20:02:44+08:00
draft = false
+++

Learned how to implement dynamic colors for Tailwind CSS in NextJS

1. put your variable in the config
2. add a style tag with this:

```
       <style>{`
    :root {
      --primary60: ${theme.primary60 ?? "var(--background)"};
      --secondary30: ${theme.secondary30 ?? "var(--secondary)"};
      --accent10: ${theme.accent10 ?? "var(--primary)"};
    }
  `}</style>
```
