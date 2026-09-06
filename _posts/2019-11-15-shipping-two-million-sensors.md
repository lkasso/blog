---
title: "Shipping two million sensors"
date: 2019-11-15 09:00:00 -0800
categories: [MbientLab]
---

I left Intel at the end of 2012 without much of a plan, which turned out to be the right amount of plan.

San Francisco was at its loudest.
People in costumes outside VC offices, meetups worth going to, bootcamp season, and dropping out of college was cool.
Everyone was riding the software vibe and startup wave.

My dad introduced me to a friend of a friend, Paul To, who had a company called Emota.
I helped him design some of the hardware for his products and got into the scene.
I made friends, and more usefully, I made relationships.

This was also the time of the iPhone explosion and the arrival of Bluetooth Low Energy (Apple was pushing hard).
What I wanted was a development platform: sensors small enough to wear that could talk to the phone in your pocket.
So I started building one, and then I started asking people whether they would actually buy it (they said yes).

I incorporated MbientLab in 2013.
I could not do it alone, so I recruited Matt and Sophie.
Stephen, Yu and Eric (ex-Intel colleagues) came later and became cofounders in everything but title.

## The Work

### MetaWear, and the Kickstarter years (2014 – 2016)

Bluetooth Low Energy · Apple · Kickstarter · Hardware

The first MetaWear went up on Kickstarter in April 2014 asking for $8,000.
It finished at **$115,067 from 1,887 backers**, a little over fourteen times the goal.
Our first customers were those backers, and a good number of them were the friends and acquaintances I had been making since 2012.

Four more campaigns followed over the next two years:

- **MetaWear RG and RPro**, April 2015. $50,622 from 590 backers.
- **MetaWear C and CPro**, August 2015. $85,977 from 1,287 backers.
- **MetaWear CEnv and CDetect**, January 2016. $53,432 from 597 backers.
- **MetaWear HR/GSR**, June 2016. $22,485 from 222 backers.

Five funded campaigns, **$327,583 from 4,583 backers**.
GigaOM called it a $30 Bluetooth module for wearables.
Make: and Fast Company picked it up too.
It was exciting.

Almost none of the product roadmap was mine.
It was dictated by what people asked for like more sensors, different form factors, coin batteries.
The MetaWear RG added a gyro.
The MetaWear Env added humidity and RGB color.
The MetaWear Detect added proximity.
We built the MetaTracker with a sturdy industrial case because customers kept putting our dev boards in places dev boards should not go.

Two did not make it.
The MetaWear HR/PPG board funded, but not by enough to actually manufacture it, so it stayed a "coming soon" on our store and then quietly stopped being one.
The MetaWear Mini, the size of a dime and meant to go into clothing, was a partnership where the partner would not fund their half.
Both were the right idea.
Neither shipped.

### MetaMotion (2016 – 2021)

10-axis IMU · Sensor fusion · NSF grants · Marketing

After the two failures we stopped chasing new categories and went back to making the existing lines better.
The MetaMotion R and MetaMotion C were supersets of the MetaWear R and MetaWear C, and they sold well for years.
MetaMotion RL and MetaMotion S came later.
By the end we had shipped thirteen distinct board models across nine generations.

In June 2016 we won an **NSF SBIR Phase I grant, $225,000**, to build cloud-based trend analysis on sensor data. We didn't get a Phase II.
It is the only outside money the company ever took that wasn't a customer paying us for something.

The market we did not plan for turned out to be research.
Our boards ended up in labs, and then in papers: **more than 160 biomedical publications in Europe PMC alone** cite MbientLab hardware, on stroke rehabilitation, gait analysis, fall detection, wearable textiles.
Robert H. Grubbs, a Nobel laureate in chemistry, used our sensors in his
research.
One 2020 *Sensors* paper benchmarks seven IMUs head to head and ours is one of them, which is a strange and gratifying thing to read about your own board.
Nestlé, BMW, UC Berkeley, Facebook, Philips, and thousands more all showed up as customers.
So did a long tail of startups we helped build prototypes, several of which went on to raise rounds far larger than anything we ever had.

What I did not expect was the range. Once you sell a small, programmable thing
that measures motion, people put it on whatever they are curious about.

- A team at Talov built [SpeakLiz](https://www.talovstudio.com/speakliz), a
  bracelet that recognizes sign language and speaks it aloud through a phone.
- Palarum built a smart sock to catch hospital falls. Blue Willow Systems, later
  part of Philips, built senior care around it. Kinemic built hands-free
  controls for railway workers. Callaghan Innovation in New Zealand used it in
  rehabilitation for partial paralysis.
- A ballet studio used it to help dancers land their turns.
- Somebody wrote a paper called [*Fitbit for Chickens?*](https://dl.acm.org/doi/pdf/10.1145/3394486.3403385),
  about mining time series from poultry to make farms more productive.
- Other people published on toothbrushing technique, cricket bowling spin rates,
  and the behavior of granular material moving through pneumatic pipes.

None of that was on the roadmap. None of it was on any roadmap.

### On the open source software (2014 – 2021)

Objective-C · C++ · Java · Swift · Python

Our software was always open source and always will be.
It is all on [GitHub](https://github.com/mbientlab).

I wrote the original Objective-C API, because I was in love with Apple and XCode was really fun and easy to use back then.
Eric wrote the C++ and Java APIs.
Stephen wrote the Swift ones.
The Python and Javascript API we wrote collectively.

Every time an API shipped or changed, we put out updated Android and iOS apps to go with it.
You can find both on the App store and the Play store today (well as of this writing anyways).

### On the contract manufacturing (2014 – 2021)

China · Encrypted firmware provisioning · Hand assembly · Customs and tariffs · Ex Works

We started contract manufacturing in the Bay Area while batches were around a thousand units.
When batches got closer to ten thousand we moved to China and stayed there.
Four separate companies handled it: one fabricated the bare PCBs, one soldered
the components onto them, one made the batteries, one made the cases.
Nothing was assembled at any of them.
The pieces came back to our own lab in California and were put together by hand.

That was deliberate.
So was the firmware.
Each unit only receives a bootloader and firmware after our test rig completes an encrypted handshake with our servers in the US.
A rig sitting on a factory floor cannot produce a working device on its own, and it cannot hand our firmware to anyone.
People tried.
We watched brute-force attempts land on the rigs and the servers.

We never shipped a bad batch and never ran a recall.
Our defect rate stayed below industry norms for the entire life of the company.

Certification was easier than people expect, but only because we knew every
piece of the product intimately, and because a small battery and a small antenna
is an easy thing to certify.
We used a lab in the Bay Area, spent real time building the test setup and fixtures, and then the testing itself took a few days and about **$10,000**.

The part I could not have done is the part Sophie did.
She forecast demand so accurately that in ten years we hit zero stock exactly once.
She worked out how to classify goods to minimize tariffs and how to route shipments to minimize freight, and she was doing this through tariff regimes and supply chain disruptions that long predate the ones people talk about now.
An absolute master of the craft.

In the lifetime of the company, we manufactured and sold **more than two and a half million sensors** worldwide.
Every single one of them passed through our own warehouse, where one of us
tested it, boxed it, and printed the label. Never a third party.

### On the team and the offices (2014 – 2021)

San Francisco · San Jose · Eight people

We started in my house in San Francisco.
Later we took an office downtown, and at our largest it held eight of us: me, Matt, Eric, Stephen, Yu, Gabriella, Mark and Sophie.
A few people came through along the way, like my friend Jesse, but that core
eight held the longest.

That was the whole company. Two and a half million units shipped, five language
SDKs, thirteen board models, Kickstarters, a federal research grant, Fortune 500
customers, and prototypes that helped other startups raise up to $50M. Eight
people.

## Exit

Then life happened.

- The team had already been thinning for years before anything else went wrong. Eric went to Amazon in 2018. Stephen stepped away to be a stay at home dad. Yu moved to Las Vegas. Every reason was a good one, and none of them were about the company.
- Then Covid. Our customers were research labs and hardware startups. Labs closed. Startup hardware budgets went first.
- We survived, barely, and we came out the other side without the money to develop new hardware.
- What was left was me, Matt, Sophie and Mark, and we moved the company to San Jose.
- The business kept running, mostly on its own. It had become an e-commerce store on life support.

That is when I took a writing job at Unit21, and MbientLab stopped being the
only thing I did.

## Takeaways

**Being a founder is lonely.** Only the people who have gone down that road
understand it, and there is no explaining it to anyone who hasn't.

**Would I do it again?** Absolutely not. I would join Nvidia and ride that wave.
But I don't regret it either. I made lifelong friends, learned lessons I could
not have learned any other way, stiffened my neck, and it led me to where I am
today.

**Work with family and friends.** People caution against it constantly. In my
experience they make excellent cofounders and they will always have your back.
The founder disputes I have watched from the outside were all between strangers.

**Hardware is hard, and the hardest part is not the engineering.** In the early
years I watched startup after startup get taken advantage of by their contract
manufacturers. Held hostage, extorted for more money before the goods would ship
out of China. Time and again these were software engineers with good degrees and
good pedigrees walking straight into the grift, and some of them did not survive
it.

## People

- [Sophie](https://www.linkedin.com/in/sophiekassovic/), a genius COO and the only reason the company ran as long as it did.
- [Matt](https://www.linkedin.com/in/matt-baker-a85744b/), the best hardware engineer I know. A genius. Cofounder and CTO.
- [Eric](https://www.linkedin.com/in/eric-tsai-6438581/), one of the two best developers I have worked with, and the kindest too.
- [Stephen](https://www.linkedin.com/in/schiffli/), the other one. If I did another startup, it would be made of five Stephens.
