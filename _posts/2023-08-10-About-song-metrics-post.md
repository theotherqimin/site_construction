---
title: "About Song Metrics"
excerpt_separator: "<!--more-->"
categories:
  - Random Projects
tags:
  - Random Projects
  - Spotify
  - Music
classes: wide
---

This whole thing started just because I really like listening to [The
Head and The
Heart](https://open.spotify.com/artist/0n94vC3S9c3mb2HyNAOcjg?si=DkJphOufQjCn6z14IhwE_g&nd=1).
I have a playlist dedicated to crying (because who likes crying in
silence? No, crying with background music is far superior) and many of
their songs feature on the playlist. If anyone cares,
[this](https://www.youtube.com/watch?v=Q8yLwuDi2mA) is my all-time
favourite performance of theirs. So back when they were releasing their
latest album ‘Every Shade of Blue’, some people started commenting about
how their ‘sound’ has changed, how they wanted music more like their
earlier albums, etc. To be fair, I think that’s the case with a lot of
artistes — some people will always like the earlier stuff more than the
newer releases and vice versa.

I don’t know if this counts as an unpopular opinion but I think people
should be allowed to not like newer songs that artistes they like put
out without being slammed or I don’t know… being called ‘fake fans’, the
same way fans shouldn’t demand artistes not change and accuse them of
being sellouts or something. Ben Howard’s old songs, for example, sound
very different from his later releases and while I prefer the old songs
([’Keep Your Head Up](https://www.youtube.com/watch?v=ADP65wbBUpc),
[‘The Fear’](https://www.youtube.com/watch?v=dnxCxHLAqn8), etc.), it
doesn’t mean I take his subsequent music as some kind of personal
betrayal.

I mean I get it, with a lot of these kinds of music, they mean
***something*** to the listener so I guess if the artist changes where
they are but you’re still back where you always were or where you want
to still be, then it kind of feels like being left behind. The songs
also mean something to the artistes though, so if they’re not where they
used to be, it’s not their fault either. I’m not sure I’m making much
sense, I’m rambling at this point. To be honest, part of this stems from
a Reddit post some years back that was talking about how at concerts,
people will yell at Ben Howard to perform his old songs even though he
has distanced himself from the first album. Again, I get that people
like the first album songs but it is also shitty to talk over and
disregard performances of the other songs, especially at their concert
(this bit shouldn’t be an unpopular opinion).

Anyway, I digress. Going back to The Head and The Heart, I do like many
of their songs, old and new, but I admit that the newer songs haven’t
been included in my crying playlist (just not the right vibes for
crying). So just for kicks, I thought I’d look at the metrics of the
tracks from the different album to see how different they are
(intuitively, I do believe that the lyric development across albums
would play a much bigger role in this story but I’m going to leave that
for another day). There isn’t much analysis here, this is purely
descriptive and there are a couple of interactive plots for you to see
specific track metrics if you’d like.

I do want to make a final point which is that having done all this, at
the end of the day, I don’t think music can/should be distilled
quantitatively like this (full disclosure: I don’t know much about
music. I don’t play any instruments, got kicked out of multiple beginner
classes when I was trying to learn though that might have more to do
with attitude than anything else, and I failed all the compulsory music
classes we used to have to take in school). All these properties
contribute to making you feel some kind of way sure, but I guess some
days I don’t want to think too much about these characteristics. Most
days I just want to [cry](https://www.youtube.com/watch?v=kdjELYZ5GbQ),
[dance](https://www.youtube.com/watch?v=hEhutIEUq8k), [feel
alive](https://www.youtube.com/watch?v=WJnrgvivZ1E), pretend I’m in a
movie [living a different
life](https://www.youtube.com/watch?v=Yam5uK6e-bQ), use it to be
[passive-aggressive](https://www.youtube.com/watch?v=yFE6qQ3ySXE) to
people (language NSFW), plan [my
wedding](https://www.youtube.com/watch?v=EmbXgoF9jEI), or [my
funeral](https://www.youtube.com/watch?v=vhd5g1Eg12k). To just feel and
not think about why (that’s the whole point of the head versus (and?)
the heart, no?)

Alright, here we go.

## Overview of albums and metrics

For the purpose of this, we’ll only use the 5 studio albums (i.e. no
live versions etc). In chronological order of release, they are ‘The
Head and The Heart’, ‘Let’s Be Still’, ‘Signs of Light’, ‘Living
Mirage’, and ‘Every Shade of Blue’. As for the metrics, we’ll use
‘valence’, ‘danceability’, ‘tempo’, and ‘energy’ from Spotify’s API. Do
I really know what the metrics are about? No (recall: failing every
music class). Will that stop me from continuing with this? No. Is that
right? Meh. I’ll talk a little bit about ‘valence’ anyway, since that
seemed the least intuitive to understand.

According to Spotify, valence is:

> A measure from 0.0 to 1.0 describing the musical positiveness conveyed
> by a track. Tracks with high valence sound more positive (e.g. happy,
> cheerful, euphoric), while tracks with low valence sound more negative
> (e.g. sad, depressed, angry).

This shouldn’t be confused for actual ‘positive-ness’ of the track. For
example, the valence of Hollywood Undead’s
[Bullet](https://www.youtube.com/watch?v=lP077RitNAc) is 0.889 but this
isn’t what the general public considers a ‘positive, uplifting’ song
(TW: self-harm/suicide). Side note: having said that, people have also
mentioned that this song helped them through difficult times, in part
because it made them feel less alone so there’s something to be said
about what’s actually ‘positive’. Again, the point is that valence
refers to how positive it sounds musically (I don’t believe it takes
into consideration lyrical content).

It’s still unclear, however, what ‘musical positiveness’ actually means.
What does it take for a track to *sound* more positive or negative? I
would have thought it would be somthing like how upbeat the song is but
it’s supposedly not about the tempo or energy of the song, since those
are separate metrics. As for the other metrics —

Danceability:

> describes how suitable a track is for dancing based on a combination
> of musical elements including tempo, rhythm stability, beat strength,
> and overall regularity. A value of 0.0 is least danceable and 1.0 is
> most danceable.

Tempo:

> The overall estimated tempo of a track in beats per minute (BPM). In
> musical terminology, tempo is the speed or pace of a given piece and
> derives directly from the average beat duration.

and Energy:

> a measure from 0.0 to 1.0 and represents a perceptual measure of
> intensity and activity. Typically, energetic tracks feel fast, loud,
> and noisy. For example, death metal has high energy, while a Bach
> prelude scores low on the scale. Perceptual features contributing to
> this attribute include dynamic range, perceived loudness, timbre,
> onset rate, and general entropy.

The chart below is an overview of the albums, the metrics and the
various relationships present.

<img src="/assets/images/posts/music_feat/unnamed-chunk-2-1.png" alt="" class="full">


The most obvious thing to note is that the number of tracks in album
increases from the earlier to latest releases (the people said ‘we want
more’ and they were like ‘okay’). Given the definition of danceability
as being, in part, based on tempo, I expected that the two would be
somewhat correlated but that doesn’t seem to be the case here. Instead,
valence is positively correlated to both danceability and energy (I
suppose it might be possible to model valence as a function of the
others to figure out what valence is…) ‘Signs of Light’ in particular
has the strongest positive correlation for both (0.909 for danceability,
0.748 for energy). With the exception of valence, the interquartile
range is also the smallest in ‘Signs of Light’ compared to the other
albums, suggesting less variability but we can take a closer look at the
tracks in each album anyway.

### Valence

<iframe src="/assets/images/posts/music_feat/valence_plot.html" height = "800px" width = "100%"></iframe>

If you hover your cursor over each point, you should be able to see the
valence for each track (of course I had to make the graph every shade of
blue. Okay well not every, just five). I greatly enjoy the fact that
across all the albums, the song with the highest valence is ‘Running
Through Hell’ while the lowest valence song is ‘Signs of Light’. I
suppose you need a bit of pep in your step while you run through hell.

### Danceability

<iframe src="/assets/images/posts/music_feat/danceability_plot.html" height = "800px" width = "100%"></iframe>

I also know nothing about dancing (does this take into consideration
specific kinds of dance? Like contemporary versus hip hop? Jazz? Can you
break dance to ‘Paradigm’? Is ‘Glory of Music II’ good for raves?)
Again, I find it hilarious that on ‘Let’s Be Still’, the track with
highest danceability is well… ‘Let’s Be Still’. In any case, it seems to
be that if you want to dance, your chances are better with the later two
albums than the earlier ones.

### Tempo

<iframe src="/assets/images/posts/music_feat/tempo_plot.html" height = "800px" width = "100%"></iframe>

This time, I included x-axis breaks at the supposedly most common tempo
markings (bpm range). Make of that what you will. It seems a little like
the variability decreases with the newer albums. Still funny to me that
slowest tempo song across all albums is wait for it… ‘Taking My Time’.
They really know what they’re doing, don’t they.

### Energy

<iframe src="/assets/images/posts/music_feat/energy_plot.html" height = "800px" width = "100%"></iframe>

Last plot here is for energy. Like before, more of the songs in the
later albums cluster near the higher end of energy while songs on the
first two albums seem more spread out. ‘Hurts (but it Goes Away)’ is the
highest energy on ‘Every Shade of Blue’, which is my favourite of that
album but ‘Rivers and Roads’, which is my favourite of ‘The Head and the
Heart’ is the lowest energy so I don’t know what that says about my
taste. Probably that I’m fickle, which is not brand new information.
They’re both just really comforting in their own way.

<br>
So that’s all for now. If I ever pull myself together to do it, there’s
probably more to unpack in the lyrics but we’ll have to wait and see if
I ever get around to doing it. It’ll probably happen when I have some
other pressing deadline to meet — that’s the best time to do other
random things.
<br><br>

#### Postscript
<p><em>I did this over a year or so ago (in bits and pieces, I kept putting
different parts of it off). Part of me did think about whether I should
still post this because it’s not great in terms of storytelling or
analytics. Code could probably also be a lot cleaner. I like to think
I’ve learned a little more since then (just a little bit) but I think
there’s value in putting rough starts out there. This took me forever in
terms of just figuring out how to connect to the Spotify API and then to
clean the data to get the five albums as they are (what with all the
multiple versions of the same song). So I guess I’m allowed to be a
little pleased that I managed it all in the end. As for having any kind
of coherent message, this was never really about the trajectory of
music, what it all means, or me trying to get better at coding. I just
wanted to be able to talk about some songs I like. Psych.</em></p>
