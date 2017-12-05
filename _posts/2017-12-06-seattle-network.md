---
layout: post
comments: true
title: "My home network: Ubiquiti Networks UniFi, Wave G Gigabit Internet, and CAT6-CAT3 wiring"
categories: [tech]
tags: [network, networking, internet, waveg]
location: "SEATTLE, WA USA"
jumbotron: true
jumbotronStyle: "background: url('//az414997.vo.msecnd.net/waz/2017network/rooftop-pano-web.jpg') no-repeat left center; background-size: cover; overflow: hidden; min-height: 500px;"
jumbotronTitle: "A photo of the Belltown neighborhood and downtown Seattle, the Space Needle, and rooftop wireless backhaul networking equipment"
---

I'm proud to live in Seattle, where affordable symmetric 1000 Mbps Internet is common in multi-family buildings and some area single-family homes, served
by a great regional network. It has been an interesting journey improving my home network over the past few years: one that I wanted to document and share in this post.

This post will be too long and will cover multiple semi-related topics:

- the Pacific Northwest network connectivity and gigabit scene
- how many condo and apartment buildings are served by Wave G (a.k.a. CondoInternet) and other regional ISPs
- my home network gear featuring the UniFi line of managed gear from Ubiquiti Networks
- challenges, including a CAT3 (yes, CAT3) home run and pulling new CAT6 in a steel/concrete construction condo

> This post is from the perspective of a tech enthusiast in Seattle: I do not represent any of the companies mentioned, and the information I have about the Seattle region's Internet providers and services is only as accurate as what I have researched and the stories I've heard.

> Full disclosure: while the initial 2 iterations of my Ubiquiti network at home were all personal investments, in October 2017 I was provided a new UniFi AC-HD access point to evaluate. I have since purchased an additional AC-HD AP at my own cost.

# Connectivity

Even today I remember the conversation with my friend Alex a decade ago when 15Mbps down and 1Mbps up was a pretty common cable Internet product offering:

> Alex: "Yeah, well, we have CondoInternet. It's symmetric 100 Mbps up and down."
> Me: "Hmm... that seems pretty hard to believe. There must be caps or something. It's not that fast. That's like university-grade."
> Alex: "Well, it's real. Also, they offer 1000Mbps up and down."

I love being 3 milliseconds away from the Westin Building Exchange, Seattle Internet Exchange and all of that lovely peering, with a 1000Mbps connection and solid gear in the rack at home.

Turns out it's real. Seattle has great Internet, and with a little more competition, it hopefully will spur some more innovation in this space. Comcast is even starting to bow to the pressure of "gigabit" and they are starting to offer gigabit and even 2Gbps services powered by DOCSIS 3.1.

## Wave G: Residential gigabit to the home

<img src="{{ site.cdn }}2017network/other-buildings.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/other-buildings2.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/cloudkeytray1.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/waveg-fiber.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/rackview.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/ubnt-wifi-hallway.jpg" class="img-responsive" title="" />

<img src="{{ site.cdn }}2017network/microfische-machine.jpg" class="img-responsive" title="" />



<img src="{{ site.cdn }}2017network/cat3-jack.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/cat6-cat3-wall-mess3.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/cat6-splicing.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/cat6-wiring-service-loop.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/ceiling-running-cables.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/closet-running-cat6.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/cloudkeytray2.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/electrical-in-ceiling.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/office-rack6.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/rack-with-sgpro.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/rooftop-microwaves.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/rooftop-waveg1.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/running-ent-through-kitchen-ceiling-walls.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/ubnt-uap-blue-night.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/ubnt-uap-wall-install.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/ubnt-wifi-bedroom.jpg" class="img-responsive" title="" />
<img src="{{ site.cdn }}2017network/ubntuap.jpg" class="img-responsive" title="" />

## Seattle: Westin Building Exchange

I still remember the disbelief when a good friend told me they had "true 100mbps Internet at home, but could upgrade to gigabit" in 2009. Their Internet service was powered by CondoInternet. Turns out I also lived in a building served by CondoInternet and so was active with the service a few hours later after a quick phone call to activate my account, where they flipped on my unit's Ethernet drop from their network closet. That was easy. Working at Microsoft I appreciate the world-class network I have access to at work, but I love that when I work from home, I have Internet that is as fast, or faster, than what I have at work, with lower latencies and a very direct connection to the Westin Building Exchange.

Techies in Seattle living in apartments and condo buildings have had blazing fast Internet for almost a decade. I am blessed to have gigabit Internet connectivity at home for the monthly cost of $80. While gigabit speeds are very common today across the region and especially worldwide, across the United States the cable monopoly and lobbyists tend to prevent any competition in this space. Wave G provides a high-value service in dense areas, essentially cashing in on customers with high expectations for connectivity and being able to cherry pick great opportunities for installations.

Today Wave G is the same service - CondoInternet (and its parent, Spectrum Networks) was acquired. Wave has also recently snatched up other niche providers in the area. CondoInternet was a boutique Seattle-area ISP serving multi-family dwellings, providing awesome connectivity, no bandwidth caps, taking advantage of the ease of wiring modern construction for Ethernet, all while monopolies like Comcast offered compartively slow, expensive services.

Since CondoInternet became available, I have lived in 3 buildings served by CondoInternet, most recently purchasing a condo a few years ago in a building with the service. I find it interesting that buildings and realtors do not more prominently advertise the availability of gigabit Internet service in the same way that Seattle Craigslist ads regularly mention "one block away from the Microsoft Connector", etc., to help draw in the tech crowd.


Westin Building Exchange
Over 200 ISPs, carriers, service providers; 19.5 MW of backup generation capacity
Rooftop line of site
34 stories tall
Hosts the Seattle Internet Exchange (SIX)
Also has lots of folks - is Equinix SE2
Next door is the relatively new Equinix SE3 facility
Largest non-commercial member-governed Internet exchange in the US; funded by donations and one-time 10Gbps port fees
Peers include Microsoft, Yahoo, Amazon, Twitter, Netflix, Google, Facebook, Peer 1, and more
http://www.datacenterknowledge.com/archives/2014/09/17/amazon-to-recycle-data-center-heat-in-seattle-offices/
https://www.westinbldg.com/Connectivity
6th and Virginia on the edge of Belltown and the Denny Triange
Datacenter heat from the building is recycled to heat Amazon's Day One/Doppler building complexes

Neighborhood also has the New York Internet (NYI) SEA1 data center on Western Ave
I believe Spectrum has fiber between WBE and NYI

60 GHz unlicensed spectrum; BridgeWave hardware; SFP; 45 watts consumption https://www.bridgewavedirect.com/wp-content/uploads/2015/10/BW64_64X_Datasheet.pdf


IPv6 Prefix Delegation /60
https://www.reddit.com/r/IAmA/comments/2m3awz/we_are_the_founders_of_condointernet_and_were/
http://www.bbpmag.com/2013mags/october/BBC_Oct13_CondoInternet.pdf
http://www.geekwire.com/2013/spectrum-wave-condointernet/
http://www.geekwire.com/2013/condointernet-expands-service-ballard/
http://www.bbpmag.com/2013mags/october/BBC_Oct13_CondoInternet.pdf
