---
title: "Home Media Server"
date: 2022-01-10T08:50:50-05:00
draft: true
---

## Some History

Now that I am coming off of my winter break, I'll finally have a chance to write about some of the things I was able to do over it. So, this post will be the first in a series of two detailing two big projects I worked on over the past 4 weeks. First, I'd like to talk about the bigger of the two projects: Rennovating my home media server. Around the summer of 2018, my Dad and I started to undertake the process of digitizing all of our media. Now, legal gray area aside, this was a success, and after almost a year of work we finally had most things digitized. Now, the goal was to eventually make everything available to the entire house. We weren't sure how to go about this, but I've heard of an application named "Kodi", so I installed a distribution of Ubuntu onto a spare computer named "Kodibuntu." This was easy enough to set up, and soon enough we had all of our songs and most of our movies stored on this machine, ready to be viewed at a moments notice.

About 6 months after this was set up, and numerous crashes from Kodi, I started looking for a different solution. I was very passive in my search, I had schoolwork to focus on as well, so this project sort of hit the backburner for a while. However, one day I was scrolling through my Google Feed and saw a github page for a project named "Jellyfin" claiming to be useful for media servers. I took a look at the project and it filled all of our boxes! Self-hosted, auto indexing software for all of our media, all while providing a central interface to get everything from. So, one weekend I tore out Kodi and replaced it with Jellyfin; after all Kodibuntu was just Ubuntu with Kodi on top of it, so I had access to all of the Ubuntu Repos. After that, it just sat there, slowly collecting any new media we got, waiting for us to watch stuff from it (which we do all the time, we have an Android TV with the Jellyfin app, we watch things on there all the time!).

## A Growing Problem

Around mid-2020, our USB DVD reader died while ripping a DVD. This was unfortunate, but it was going on 3 years old at this point, it was probably its time. So, we decided it was time to upgrade. We ended up buying a USB Bluray drive so we could begin to rip HD and UHD content to our media server; I mean, the TV we had downstairs was a UHD TV, it was time to stop watching 480p DVDs on it. We had a 1TB drive installed from the beginning, and we were only using about 150GB thus far, so we figured we still had a while before it ran out. That was before we ripped out first blu-ray disc. It ended up being around 30GB after we got done ripping, and after compressing the video further in handbrake it we got it to around 20GB. The Ultra HD Blu-ray discs were closer to 50GB! So, our estimate on how long the server would last quickly dropped.

While we *were* using more space quickly, we still never surpassed 1TB. This wouldn't happen for another year or so. Around the fall of 2020, I left for college, and as things began to open up more permanently buying and ripping movies started to fall to the wayside once again. We had spurts of buying and ripping discs, but nothing too often. However, we were starting to run into issues streaming out UHD content. It would buffer quite often. We figured this was a sympotom of our WIFI link being slow, but in hindsight this may not have been the case. We've been wanting to upgrade the machine for a while, but never had any reason (or the time) to do so just yet. My dad brought home a decomissioned server from his office that had 6 1TB drives in it. One day we'd move everything over, but now wasn't the time.

## A Breaking Point

Just this past Christmas (2021), we ran into a breaking point. I was gifted a box set containing the full series of *The Office* (because it was taken off of Netflix for the sole reason of promoting Peacock, so I refuse to use Peacock), so I wanted to put it on the server before I left for college again. I got through about 3 seasons until I noticed the size of the folder: 250GB! This was huge, and I still had 6 seasons to go, probably was going to be around 850-900GB of content in total. This was never going to fit on the current server, which probably had about 90GB still free on it. We had to finally implement this new server. However, we didn't want to do it haphazardly. We were going to do this right (or at least as right as we know how).

## Planning the Solution

So, we had this server that had a total of 6TB of storage and 32GB of RAM. This was *more* than enough for our needs. Since we were also looking to overhaul our home network, we decided to work on this as well.
