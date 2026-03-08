# Microservices: How Big Companies Use Them (and Sometimes Don't)

---

## 1. How Netflix Uses Microservices

Think of microservices like a restaurant kitchen — instead of one chef doing everything, you have separate people handling salads, grilling, desserts, and so on. Netflix works the same way.

Back in 2008, Netflix had one big system running everything together. When part of it broke, the *entire* service went down for three days. That was a wake-up call. Netflix spent the next several years breaking their big system into **over 1,000 small, independent services** — each one doing just one job, like logging you in, recommending shows, or processing payments.

If one service has a problem, the rest keep working. So if the recommendations feature breaks, you can still press play and watch your show. Each service can also be updated or scaled up on its own — for example, when a popular new show drops and millions of people log in at once, Netflix can boost just the streaming service without touching anything else.

---

## 2. Two Other Companies Using Microservices

### Uber
When Uber started, it was just one app for one city. Their code was all in one place — easy to manage for a small team. But as Uber grew to hundreds of cities and millions of rides, that single codebase became a nightmare. Making one small change could accidentally break something else, and new developers were scared to touch anything.

So Uber split things up: one service for matching riders to drivers, one for payments, one for trip tracking, and so on. Different teams now own different services and can work independently. This made Uber much faster at releasing updates and fixing bugs. At its peak, Uber was running over **1,300 microservices** — which actually got a bit too complicated, but it still worked far better than one giant system.

### Amazon
Amazon faced the same growing pains around 2001. Their shopping website was one huge system, and with hundreds of engineers all working in it, deploying even a small update could take weeks because everything was tangled together. Amazon separated their system into independent services — product search, shopping cart, checkout, recommendations, and more. Teams could now work and deploy on their own without waiting for everyone else. This experience was so valuable that it directly inspired Amazon to build **AWS**, so other companies could use the same kind of infrastructure.

---

## 3. Companies That Switched Back to a Single System (Monolith)

Sometimes microservices cause more problems than they solve. Here are two companies that decided to go back to a simpler approach.

### Amazon Prime Video
In 2023, the Prime Video team shared a surprising story. They had built their video quality monitoring tool as a set of microservices — separate little programs passing data back and forth. But it turned out to be slow, expensive, and hit a wall when they tried to scale it up. They merged everything back into one program running in one place, and their costs dropped by **90%**. The lesson: microservices aren't always the right tool, even at a big company like Amazon.

### Shopify
Shopify also pulled back from microservices. Managing dozens of separate services meant a lot of extra work — tracking down bugs was hard when a problem could be hiding in any one of many services, and coordinating updates across teams became slow and complicated. They moved toward a simpler "all-in-one" structure that was easier to work with, while still keeping things organized internally.

