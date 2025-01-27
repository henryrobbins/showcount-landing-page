---
layout: update
title:  "A New Project"
date:   2025-01-26 22:00:00 -0400
hidden: true
categories:
---

I'm starting a new project: showcount.com. In short, it's a jam-band-centric social media platform for people to track and share their shows.

The jam scene is blessed with a number of incredible platforms. Looking for tickets? [CashOrTrade][cashortrade]. Live music news? [Relix][relix] and [JamBase][jambase]. Fresh tapes? [Nugs][nugs] and [Internet Archive][internet-archive]. Setlists? [Songfish][songfish] and [setlist.fm][setlist.fm]. However, I've yet to come across a platform that allows concert tracking and sharing. That's the hole I intend for showcount.com to fill.

## Songfish

Songfish comes the closest to a concert tracking and sharing platform. You've probably used Songfish even if you haven't heard of it. Created by Adam Scheinberg, Songfish is the setlist engine powering [All Things Umphrey's (ATU)][allthings], [Phish.net][phish.net], and [El Goose.net][elgoose.net] among many others. If you want the source-of-truth for your band's setlists, you better hope they're on Songfish. In addition to poring over a band's setlists and stats, Songfish allows one to create their own show lists to track personal stats. It's great. I've been tracking my Umphrey's shows since 2016.

However, there are two features Songfish lacks that I've come to miss. First, I don't know many people in the jam scene that only see one band. I don't want my show tracking to be fragmented across all the bands I see. I know many others who feel the same and the solution most of them have turned to is an Excel spreadsheet. That's a real shame because I want to see what they're up to! Second, user interfaces inherently limit the ways you can slice and dice data. Thus, if you want to view a unique stat that isn't available, you need direct access to the data. The [All Things Umphrey's API][allthings-api] (provided by Songfish) was an awesome step in this direction, but still falls short of fully flexible access. I expect the number of people who this second feature applies to is much smaller. But, I'm one of them.

## Past Projects

This isn't my first time thinking about this. I've had two previous related projects: Umphbase, a Deadbase inspired reference book of Umphrey's McGee setlists and love-music-will-travel, my personal show-tracking website.

### Umphbase

When my dad showed me his old copies of Deadbase (his copy of IV is on the shelf behind me), my first thought was, "Damn, how does Umphrey's not have this?" I liked the physicality of it, but there were also so many great stats I couldn't view on ATU. I remember being particularly bummed I couldn't see the song and transition before / after in the "Every Time Played" section (funny enough, that's now been added in Songfish).

In December 2020, I wrote code to scrape all the setlists from ATU and load them into my own database. With my own database of Umphrey's setlists, I then compiled a Deadbase-like reference book I called [Umphbase][umphbase]. [Here][umphbase-pdf] was the first version. After that, the project lost momentum (the Spring semester started).

I picked things back up in Summer 2021 when I saw that Adam had added the [All Things Umphrey's API][allthings-api]. This made getting all of the setlist information infinitely easier (though still not without challenge). This time around, I spun up a service that checked ATU for new setlists every day and continually updated the database. I also made publicly available a link to download the entire setlist database. I've since taken it down as it cost $20/month to keep up. Again, the project lost momentum (the Fall semester started).

The last time I revisited the project was in December 2021. I refined the book compilation and had some fun with automatic song code generation. Deadbase assigned unique 4-character codes to every song the Grateful Dead played. In Deadbase IV, there are about 250 songs. Umphrey's provided a unique challenge with nearly *1,000 songs*. Below are some samples from the latest compilation.

<div class="iframe-container">
<iframe src="/assets/updates/2025-01-26-a-new-project/every_time_played.pdf#toolbar=0" width="80%" height="400px"></iframe><br>
<iframe src="/assets/updates/2025-01-26-a-new-project/song_codes.pdf#toolbar=0" width="80%" height="400px"></iframe><br>
<iframe src="/assets/updates/2025-01-26-a-new-project/songs_played.pdf#toolbar=0" width="80%" height="400px"></iframe><br>
<iframe src="/assets/updates/2025-01-26-a-new-project/jimmy_stewarts.pdf#toolbar=0" width="80%" height="400px"></iframe>
</div>

Despite being idle for 3+ years, the book isn't closed on Umphbase yet. It's had an important piece missing from the beginning, one I'm hopeful showcount.com is a step towards resolving. One of, if not the greatest, features of Deadbase is the "Feedback" section which outlines the results of questionnaire responses. This had everything from "When was your first Dead concert?" to "Do you maintain a current tape list? If so, what sort of rating system do you use? Numeric (1-7), Grade (A-), Words (vg)." The show reviews and venue ratings offer valuable insights. Conversely, the arena survey asking venues how Dead Head behavior compared to their other venue attendees is just hilarious. I aim for showcount.com to be a forum where this data can be collected for Umphrey's, among other jam bands.

### love-music-will-travel

I retroactively pulled together all the concerts I'd ever attended in early 2022 from old ticket stubs, emails, photos, and anything else that might have left a clue. I've been tracking every show I attend ever since. In November 2022, I decided to make a website to share the shows I'd attended.

<!-- TODO (hwr): Finish update -->

<!-- Projects -->
[love-music-will-travel]: https://love-music-will-travel.henryrobbins.com/
[umphbase]: https://github.com/henryrobbins/umphbase
[umphbase-pdf]: https://github.com/henryrobbins/umphbase/blob/master/v1.0.0/umphbase-v1.0.0/umphbase-v1.0.0.pdf

<!-- Platforms -->
[r/jambands]: https://www.reddit.com/r/jambands/
[relix]: https://relix.com/
[jambase]: https://www.jambase.com/
[songfish]: https://songfishapp.com/
[cashortrade]: https://cashortrade.org/
[nugs]: https://www.nugs.net/
[internet-archive]: https://web.archive.org/
[setlist.fm]: https://www.setlist.fm/setlists

<!-- Songfish setlist sites -->
[allthings]: https://allthings.umphreys.com/
[allthings-api]: https://allthings.umphreys.com/api/docs#void
[phish.net]: https://phish.net/setlists/phish/
[elgoose.net]: https://elgoose.net/setlists/
