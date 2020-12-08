+++ 
draft = false
date = 2020-10-02T05:23:08-05:00
title = "Building a Space Elevator"
description = "How to build the tallest structure possible."
slug = "building-a-space-elevator" 
tags = ['space','elevator']
categories = ['innovation']
externalLink = ""
series = []
+++

# Introduction

[this post has been edited](https://github.com/heroLFG/hugo-herolfg-site/commits/dev/content/posts/space-elevator.md)

The space elevator is a kind of structure which connects the surface of a large gravitational body with space.  The tallest buildings on Earth are not space elevators and there are challenges we face when we construct tall buildings.  I have discovered an architecture for overcoming these engineering challenges which divides the load using partitioning.

The tallest structure possible must make use of forces like buoyancy which oppose gravity.  I will explain the architecture in the most simple way using a thought experiment.  Create a helium balloon and tie it to the longest string possible.  At some point the downward gravitational force of the system will exceed the upward buoyant force of the helium balloon.  This buoyant system can be considered as a link in a chain of similar buoyant systems.  The end of the string on each link is connected to another balloon on another link.  We now have the ability to create a vertical structure which is taller than Mount Everest.

There are limits to the strategy of using a balloon because the buoyant force decreases as the balloon rises in the atmosphere.  The links which will be highest can have less string.  Other kinds of forces which oppose gravity could be used to account for this fact and reach greater heights.

Another way I have imagined this vertical structure is by creating a quadcopter that is tethered to a power cord and creates a link in a chain similar to how we imagined the chain of balloons and strings.  The difference between the quadcopter and power cord link is that you can begin to construct a vertical structure that looks very much like a power distribution system we use in the power grid today.  In this thought experiment of mechanized flying objects connected in a chain which forms a power distribution circuit I have thought it necessary to tether this vertical structure to a reliable power source.

I shared this space elevator idea on [youtube](https://www.youtube.com/watch?v=WEmPVD8GNbU) in 2015.  I tried to share this idea with Elon Musk and Jeff Bezos because they seem to be interested in big ideas and getting into space.  My thinking is rooted in a submission I made to the National Science Foundation which would empty and refill a body of water using the least amount of energy through this kind of sharing work via a partitioning strategy.

{{< youtube WEmPVD8GNbU >}}

# Some Math

## Assume We Have a Nuclear Reactor

How much electricity does a nuclear [power plant generate](https://www.eia.gov/tools/faqs/faq.php?id=104&t=3)?

> The Palo Verde nuclear power plant in Arizona is the largest nuclear power plant in the United States with three reactors and a total net summer electricity generating capacity of about `3,937 MW`

How many large drones can we service with this nuclear power plant if we ignore the mass of the power grid used to service the drones?

I found that DJI has some Agras model aircraft for agriculture use.  They have a takeoff weight of `23 kg` and can remain in the air for about `10 minutes` using a `12,000 mAh` battery at `44.4 V`.  This is a `532.8 Wh` battery dervied from the equation `Volts * Amp-hours = Watt-hours`.  A `532.8 W` aircraft would have flown for 1 hour on this battery.  But this aircraft flew for 10 minutes.  Therefore, this aircraft uses `3196.8 W`.

We can now get an estimate for the total number of aircraft which can be powered by this nuclear power plant:
`3,937,000,000 / 3,196.8 = 1,231,544.04 drones`

If each drone were about 1 meter apart, then the structure could extend to over 1200 km away from the Earth's surface.  To put this in perspective, the International Space Station is an average of 400 km away from the Earth's surface.

### notes
- These calculations do not consider the mass of the power grid which would need to be suspended in air by the swarm of drones.
- The drone I looked at has a service ceiling of 2 km.