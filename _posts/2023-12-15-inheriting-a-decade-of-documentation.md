---
title: "Inheriting a decade of documentation"
date: 2023-12-15
categories: [Gradle]
---

This one is still going, so this is only the first year of it.

I was on my way out of Unit21 in a layoff and already interviewing when Gradle came up on LinkedIn.
They wanted someone who could write and who knew Gradle, which is a narrow enough intersection that I thought I had a real chance.

I did know Gradle, in the way most people know Gradle.
I had used it building Android apps at MbientLab, where it was the part of the process that sits between you and the thing you actually want to do.
A build file you edit when something breaks.
Little did I know.

The interview process was long.
Justin interviewed me, and so did Piotr, who is still my boss.
I remember Piotr ended up talking to my ex Unit21 boss, Andrew, for over an hour.
I joined in January 2023 as a technical writer, not a lead or an advocate.
That came later.

## The Work

<div class="era" markdown="1">

### What I inherited (January 2023)

Asciidoctor · Javadoc · Dokka · Markdown

There had been a writer before me, but he was long gone when I got there, and he had not been technical.
He supported the engineers rather than owning the documentation.
So in practice the docs had been written by engineers, when they felt like it or when they had to, for about a decade.

That produces a very particular kind of documentation.
The subject matter was good.
The people writing it knew more about Gradle than anyone alive.
It had gaps, though, and it was written for people who already understood Gradle.

The numbers back that up more starkly than I expected.
The user guide had 165 source pages in November 2022 and 166 when Gradle 8.0 shipped in February 2023.
One page, in a year.
Those pages were getting over a million visits a month.

Gradle 8.0 landed about a month after I did.
Luckily it did not land on me.
I needed the time to ramp up.

I also felt like I was paying the price of my predecessor's failure, and I was under more scrutiny and micromanagement than I had ever been in my life.

</div>

<div class="era" markdown="1">

### The Develocity detour (first half of 2023)

When I joined I was also asked to take on the documentation for Gradle Enterprise, the commercial product, which was renamed Develocity that September.

I said yes happily.
It took about six months to become obvious that this was not one job with some extra scope, it was two jobs.
Luckily we hired someone on the Develocity side to do it properly, which was the right call.

I suffered for a bit though.

</div>

<div class="era" markdown="1">

### Rebuilding for beginners (August – November 2023)

Information architecture · Getting Started · Core Concepts

Everything I changed that year came back to one problem: the documentation assumed you already knew Gradle.

It shipped in two waves, both tied to releases.

Gradle 8.3, August 2023.
The flat cluster of Quick Start, Getting Started, Installing and Samples became a single numbered Getting Started tutorial that runs in order.
If you have never used Gradle, there is now one path through the front door rather than four half-open ones.

Gradle 8.5, November 2023.
The bigger one.
I split the manual into two parallel tracks, running Gradle builds and authoring them, each with a Core Concepts sequence and a tutorial sequence.
That is still the shape of the documentation today.

The landing page changed too.
It had been a table of contents pretending to be a page.
It became something written.

I also added a rating widget so readers could score a page.
The scores were low at first, which was demoralizing in a way I had not braced for.
Over time I got them up by about 40%.
I took the widget out last year and put the attention into GitHub issues instead, which turned out to be a better signal.

By the end of 2023 the user guide was 202 pages.
Thirty-six more than the year had started with, against one page the year before.

</div>

<div class="era" markdown="1">

### Working in the open (2023)

GitHub · Asciidoctor · DCO · Contributor guidelines

Gradle's documentation lives inside the `gradle/gradle` repository, in Asciidoctor, alongside the code.
Every change is a pull request in a repo that thousands of developers watch.

I love this, and I did not expect to.
There is the GitHub credibility of it, and there is the community, which is genuinely good.
External contributors send documentation pull requests constantly, and they are good pull requests.
That still surprises people when I tell them.

I am tagged automatically on anything touching docs, and I can block a change.
Engineers on the team can override me, which happens rarely.
The American English rule predates me.
A lot of the contributor guidelines in there now do not.

</div>

## Takeaways

**Gradle is hard, and I underestimated it completely.**
I had used it for years and thought of it as a step in a build.
It took me about two years to feel properly ramped up.
The gap between using a tool and being able to explain it is much wider than it looks from the outside.

**The hardest part of inheriting a decade of anything is deciding what to keep.**
Almost none of what I found was wrong.
It was incomplete, and it was addressed to the wrong reader.
Those are different problems from bad writing and they need different fixes.

**There are too many ways to do one thing in Gradle.**
I try to hold a line on keeping it simple.
It is harder than it sounds when every one of those ways is somebody's legitimate use case.

**Do it yourself.**
My entire team is in another time zone.
Waiting for an answer costs you a day, so mostly I learn the thing and get on with it.
I picked that habit up running my own company and it has been the single most useful one here.

## People

- [Tom](https://www.linkedin.com/in/tom-t-373ba0b/), my best and harshest critic, and a genius at what he does.
- [Piotr](https://www.linkedin.com/in/piotr-jagielski-1416b623/), who interviewed me and is still my boss, and a great one.
- [Justin](https://www.linkedin.com/in/justin-van-dort/), who somehow still puts up with me.
- [Louis](https://www.linkedin.com/in/ljacomet/), my manager when my manager is not around.
- [Sterling](https://www.linkedin.com/in/sterlinggreene/), who keeps me grounded when I am making decisions about the docs.
