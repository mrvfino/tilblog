+++
title = 'Day 27: Finding and Working Around a Bug in Alamofire (or Moya?)'
date = 2024-02-24T21:54:19+08:00
draft = false
+++

While working on a batch POST feature on an app, I encountered an odd bug while using (Moya)[https://github.com/Moya/Moya]. It's easier to understand when explained step by step:

Goal: The goal is to call multiple POST requests on an endpoint.

1. Create an array of Observables for each POST requests.
2. Combine merge the Observables using ".merge"
3. Trigger the cancellable.

If you're thinking that it would submit each individually, to my surprise it didn't. Which was very strange to me because I've already implemented this feature twice in the same app, and has been battletested by hundred of users already. So what went wrong?

Luckily I found the discrepancy.

It was the paths of these APIs. The path pattern of the working batch POST features follow a `foo/{id}/bar` pattern while the bugged one was only `bar`. I couldn't really believe it at first and almost didn't bother to look into it further but it was the only differentiator between the three, and I'm running out of time.

Luckily I had a working assumption.

Disclaimer, I don't know how Alamofire or Moya exactly works under the hood. So looking at it fundamentally, I just thought to myself that if I were to implement a feature to track multiple requests at a time, I'd need a key-value store to do so. And if Alamofire / Moya implements a similar way.
