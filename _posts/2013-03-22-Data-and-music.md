---
layout: page
title: Data and music
---

# {{ page.title }}

## 22 March 2013 - Kev Kirkland

Saw an interesting talk at Pervasive Media Labs about real time sensors. X-io have designed a board which broadcasts data for the 'music gloves' used by Imogen Heap (amongst other things, see http://www.x-io.co.uk/).

A chat with Verity afterwards opened up the discussion of non-visual representations of data. In the same way that we can animate data changing over time (e.g. see <a href="http://www.gapminder.org/world/#$majorMode=chart$is;shi=t;ly=2003;lb=f;il=t;fs=11;al=30;stl=t;st=t;nsl=t;se=t$wst;tts=C$ts;sp=5.59290322580644;ti=1822$zpv;v=0$inc_x;mmid=XCOORDS;iid=phAwcNAVuyj1jiMAkmq1iMg;by=ind$inc_y;mmid=YCOORDS;iid=phAwcNAVuyj2tPLxKvvnNPA;by=ind$inc_s;uniValue=8.21;iid=phAwcNAVuyj0XOoBL_n5tAQ;by=ind$inc_c;uniValue=255;gid=CATID0;by=grp$map_x;scale=log;dataMin=283;dataMax=110808$map_y;scale=lin;dataMin=18;dataMax=87$map_s;sma=49;smi=2.65$cd;bd=0$inds=;modified=75" target="_blank">GapMinder</a>), we can animate sounds over time. Given a lot of people prefer processing audio information, it's worth looking into. I couldn't think of many ways that data has been expressed with sound. I guess the classic example would be a geiger counter, where proximity to radiation is mapped to a pitch - highly informative (but not destined to become a best seller).

This might work for detecting correlation. For example you could map the price house in an area to a sound which changes pitch according to how high the price is, and another sound mapped to the average life expectancy (perhaps with a mean sound as well for a reference point). Each area would have a different 'song'. It would be an interesting experiment to see if listeners pick up any different patterns than those seen in a visualisation. When looking at a picture we have the freedom to jump to any point which looks interesting, but do we miss any other subtle patterns because of this? Would a linear form like sounds/music give us an insight into other patterns?

One danger is that disonance (e.g. when the difference in pitch between mapped data points becomes a flattened 5th) might make the relationship sound 'bad' when it could indicate a positive relationship in the data. The representation of sound already has a 'meaning' other than the value we've given it for the data. It would probably make sense to map the data points to some other kind of filter that's applied to a constant motif instead to try to mitigate this.
