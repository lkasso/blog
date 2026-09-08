---
title: "Validating and designing silicon at Intel"
date: 2012-12-14
categories: [Intel]
---

It was the end of my junior year at Purdue, studying electrical engineering, and the start of the summer of 2008.
I was fortunate enough to spend that as an intern on Intel's post-silicon validation team.
There was one full-time headcount waiting at the end of the internship and two of us interning for it.
The other intern was genuinely good, and she became a friend, which did not help.
I worked hard and I won it.

Winning it and getting it turned out to be two different things.
2009 was a bad year to be competing for a single opening, and Intel offered the role to another woman graduating in my year.
She was simply that good.
She turned it down for AMD, went to Oracle after that, and remains one of the engineers I most admire in this field.

Which is how I came to turn down my own offer from GE's locomotive division and move to Folsom, California.
I have Skip Lindsay to thank for that, a damn good Principal Engineer, my recruiter, and still the best manager I have worked for.

## The Work

<div class="era" markdown="1">

### Post Silicon Validation Engineer (2009 – 2011)

x86 microarchitecture · RTL emulation · FPGAs · Perl

The job was debugging microarchitectural sightings, both on physical systems and in RTL emulation environments, and building the tooling that made that debugging possible.
I worked across Sandy Bridge and Ivy Bridge, and across a wide set of IPs: CPU core, system agent, power management, microcode.

Most of it came down to a loop.
A failure happens in silicon, and we had a backdoor that captured the state of the machine right before it went wrong.
You replay that state on emulators and FPGAs, and then you find the bug by walking the system forward in slow time.
And you cross your fingers that you know the system well enough, and are lucky enough to catch the failure in the act, to fix it at all.

</div>

<div class="era" markdown="1">

### Component Design Engineer (2011 – 2012)

SystemVerilog · DDR PHY · DFI & LPDDR protocols · mixed-signal design · lint/CDC/RDC

I moved to the MOD MEM team and to the other side of the fence, doing logic design for the DDR PHY on Atom-based SoCs instead of validating someone else's work.

The job ran from defining the microarchitecture of a block, through implementing it in SystemVerilog, to holding the RTL to the front-end quality bars:
lint, clock and reset domain crossings, voltage domain crossings, synthesis checks.
Code and test. Code and test. And then more tests.
Memory I/O is mixed-signal and it lives on a power budget, so area and power optimization was never a later phase.

The funniest part of my last year at Intel was moving my team off SVN and onto Git.
Engineers can be notoriously pig-headed about new tooling, so I wrote a course on Git and made access to the codebase contingent on taking it.
If you would not do the course and show some willingness to learn the thing, your credentials stopped working.
Yes, it was a bit passive-aggressive.
Git was still unfamiliar to most of the team back then, and I hope they look back on it as a good memory, and a great skill to have.

</div>

## Exit

- I was promoted on the validation team.
- On the design team, the next promotion was declined. Not on the strength of
  the work. The reason given was that promoting someone twice in a row was not
  how things were done, and at Intel then, it more or less wasn't.
- I did not want to spend the next several years inside a culture that treated
  that as a sufficient reason.
- Startups were becoming the obvious alternative, and I wanted to find out what
  that was like. I left at the end of 2012 and started MbientLab the following
  year.

## Takeaways

**VLSI was my dream job.** Then I got it. The thing I had been certain I wanted
to do for the rest of my life turned out not to hold me once I was actually
doing it, and that is a strange and useful thing to learn early.

**Big company culture has to be experienced.** Nothing prepares you for the
scale, the process, or the number of people who have to agree before anything
moves. I am glad I have four years of it in me, and I would not trade them, even
knowing how it ended.

**Intel's Principal Engineers are some of the smartest people in the world.** I
mean that without qualification. Watching how they took a problem apart changed
how I take problems apart.

I also got to travel to and work in Israel, which was not something I had
expected the job to include.

## People

- [Skip](https://www.linkedin.com/in/william-c-lindsay-07a5a6a3/) hired
  me out of that internship and set the bar for every manager since.
- [Josh](https://www.linkedin.com/in/josh-pfrimmer-50336b75/) was one of
  the best mentors I have had, and the person who got me into rock climbing.
- [Keerthi](https://www.linkedin.com/in/keerthi-r-patlolla-7a070811/)
  was a wonderful colleague and made the day-to-day better.
