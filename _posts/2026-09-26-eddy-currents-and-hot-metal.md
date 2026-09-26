---
title: "Eddy currents and hot metal"
date: 2026-09-26
categories: [Beacon]
---

Matt was always deep in 3D printing, and he had a problem he could not stop thinking about: getting a perfect first layer, every time, on any bed.
Every probe on the market solved it mechanically, so your accuracy was bounded by how precisely you could build a moving part.

His idea was to take the moving parts out of it.
Measure the distance electrically instead, and you are working in microns rather than millimeters.

## The Work

<div class="era" markdown="1">

### Getting to a product (2020 – 2023)

Eddy current · Klipper · Rust

It started during COVID as something Matt did in the evenings, and it took years to become a thing you could buy.

The version we shipped was called RevD, which tells you there were a RevA, a RevB and a RevC before it.
Some of those redesigns were ours and some were forced on us: this was the chip shortage, and parts we had designed around simply stopped existing.
Mostly it cost time, because Matt was doing it part time.

[Annex Engineering](https://github.com/Annex-Engineering) helped it over the line, with software, with testing, and later with support.
[Dalegaard](https://www.linkedin.com/in/dalegaard/) did the work that made Matt's hardware actually speak Klipper, and he is a pure genius.
He is only visible on GitHub, in the copyright header of the module, because that is where the work is.
The store and the site are the part Matt and I built.

Beacon launched on 6 February 2023.

</div>

<div class="era" markdown="1">

### Eddy currents and hot metal (2023)

Thermal compensation · Coil design · PCB materials

An eddy current sensor works by driving a coil at high frequency, inducing currents in the metal underneath, and measuring how that loads the coil.
The reading depends on the coil's own inductance and resistance, and on the conductivity of the metal it is looking at.

Every one of those moves with temperature.
And the sensor is bolted to a toolhead a few millimeters above a bed held at 60 to 110 degrees, soaking, for the entire print.
So the zero wanders.
On a 0.2mm layer, a few microns of wander is a first layer you can see.

It was really bad at first.
The fix was not clever, it was expensive: a great deal of testing, and our own thermal compensation algorithm built from it.

RevH, at the end of 2023, attacked the same problem in the hardware.
A redesigned coil, smarter PCB materials, a better shape.
That bought about 40% less thermal drift and around 20% more sensitivity, and added an accelerometer on board so the same part could do input shaping.

</div>

<div class="era" markdown="1">

### Contact (2024)

Firmware 2.0.0 · TrueZero

Contact was Matt's idea and it is the thing I would point people at.

The sensor is reading distance continuously at 1kHz.
So if you drive the nozzle slowly down into the bed, you do not need a strain gauge or a switch to know when it touches.
You just watch the distance signal stop changing.
The nozzle has arrived.
No moving parts, no added hardware, and it works on surfaces that are no good for scanning.

We did not ship it until it could find an egg without breaking the egg.
That went in the release video.

It also carries the bluntest warning in our documentation, that a misconfiguration could ruin your day and you use it at your own risk.
That language is there because people misconfigured it and drove nozzles into their build surfaces.
We felt terrible.
There was not much we could do except say so plainly.

</div>

<div class="era" markdown="1">

### Support that lives somewhere else (2023 – 2026)

Discord · Open source · DIY

Beacon has never had a support desk.
Technical questions go to Annex Engineering's Discord, which is not ours.

That was not a philosophy, it was arithmetic.
Two people cannot support thousands of customers, and we had friends who already ran the room those customers were in.

The 3D printing community is open source and DIY by disposition.
They design their own toolhead mounts and publish them.
They expect to do some of the work.
That is a different relationship with a customer than the one I ended up in at MbientLab, and it is better.

Not everything about it is comfortable.
The real complaints are fair: we are more expensive than the alternatives, the cable is fragile and not rated for routing in a chain, and certain single-board computers have USB power designs that will damage a Beacon, which is why our product pages tell you not to use them.

</div>

## Where it stands

- Beacon still works, still sells, and still has stock.
- We are going to run the inventory down and then stop. Probably next year.
- Same two people, same ending as MbientLab, for mostly the same reasons.
- The Klipper module is GPL-3.0 and stays where it is.

## Takeaways

**Electrical beats mechanical when you need microns.**
That was the whole insight and it was Matt's.
Everything else was execution.

**Physics does not care about your schedule.**
The solution to the thermal drift problem was long, boring and expensive: test until we understood it, then compensate for what we had measured.

**Releasing something when it works on an egg is a good rule.**
Pick the test that would embarrass you to fail, and do not ship until you pass it.

**Open source means someone else gets to build on it.**
We released the Klipper module under the GPL, so a competitor can take that work, attribute it, and undercut us with it, because they did not pay for the years of R&D that produced it.
That is exactly what the license allows.
Knowing it was coming does not make it feel good, and I would still release it the same way.
