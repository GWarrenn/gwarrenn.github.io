---
layout: post_wider
title: "2000: A Cycling Odyssey" 
---

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/master/images/cycling_odyssey/fancy_horse.png)

For 2019, I decided to set a goal: bike 2000 miles over the course of the year. In order to keep myself accountable, I decided that I would make some public facing visualizations using Strava data to publicly shame/reward me for my progress. Then, another idea came to mind: what if I set up a betting market around my progress? I decided that I would turn myself into a fancy racehorse and let people try to guess how much progress I will have made towards my goal as of December 31st, 2019. At the end of the year the top three will receive a share of the pot. I will also donate a share of the pool towards a charity of choice.

In order to allow gamblers keep track of their bets, I've built the following progress tracking visualization, which processes scraped data from my [Strava account](https://www.strava.com/athletes/4778598). The visualization on the left shows my cumulative progress as a percentage of 2000 miles alongside a diagonal reference line showing a consistent pace needed to hit 2000 miles within a year. The visualization on the right plots the average speed and total distance of each bike ride throughout the year. Strava allows users to tag certain rides as commutes, which I've coded in the lighter colors, while the darker dots represent longer, performance-oriented rides. The process isn't entirely live/automated because the security protocol the Strava API uses and technical limitations on my part, so there may be a bit of a lag in reporting.

<figure class="video_container">
<iframe width="2000" height="700" src="https://raw.githack.com/GWarrenn/fancy-racehorse/master/index.html" frameborder="0" allowfullscreen="true"></iframe>
</figure>

Some Ground Rules
--------------

1. One entry/bet is $5. The initial betting will only be open until March 1st. You can make a guess without betting money, but in that case all that you win will be the satisfaction of being right and the payout will go to the next closest guess.

2. The person with the closest bet to the actual outcome as of December 31st, 2019 at 11:59:59 eastern time (without going over) will be declared the winner. In the event of a tie, the winners will split the winnings. So if five people pick the same winning number, they all split the first place prize. It might be wise to avoid common numbers that others might pick (ie 500, 1000, 1500). Or, now that I've said this and no one will pick them, maybe you SHOULD pick them!

3. Obviously, you can guess as high or low as you want. I don't plan on stopping for the year if I hit 2000 miles, but there is obviously a limitation on my frail human body.

4. You can enter as many guesses as you want. If you decide to enter more than one guess, but only bet money on one guess, you must specify which guess is attached to the bet. 

5. Payouts are as follows, once the pool is closed and all bets are collected the percentages will be updated with actual dollar amounts.

	* 1st place: 50%
	* 2nd place: 15%
	* 3rd place: 10%
	* Charity ([Women Involved in Reentry Efforts (The WIRE)](https://thewiredc.org/)): 25%

6. I will not see any of the bets until the year is over, as I want to minimize any bias in how I ride. 

7. If I sustain any injuries throughout the year that would keep me off my bike for longer than a month, all bets are off; you will be refunded your original bet and I will donate the money to charity myself.

If there is sufficient interest, there may be monthly pools, where you all will have the opportunity to bet on monthly distances in addition to the yearly bet.

About This Fancy Racehorse
--------------

In order to allow people to make a somewhat informed bet, I'll give some background as to my biking experience, general physical fitness, and social habits.

I'm 28 years old and I've been biking for the past 8 years. I ride a 2014 Trek 1.5C, which has seen a good amount of mileage over the years, serving as my commuting and long-distance bike.

In previous years, I've undertaken some longer rides, including two 100 mile rides ([like this one](https://www.strava.com/activities/337245565) & [this one](https://www.strava.com/activities/159745215)). I hope to work up to another century this year, but a "normal" weekend ride for me will generally range between 20 & 50 miles.

I work a traditional 9 to 5 office job within DC, where I also live. On most days, when the weather isn't too terrible and I'm feeling up for it, I'll bike to and from work, which is about 8 miles round trip. In the past, I haven't recorded these activities because it's such a short ride, but I will be counting these rides towards the total this year (Sorry in advance if you're one of the few people that follow me on Strava)

Outside of biking, I play in a somewhat competitive 11 v. 11 soccer league, which takes place year-round every Saturday morning with a few weeks off between seasons. 

Obviously, you're reading this on my personal blog. In addition to my day job, I also spend a fair amount of my personal time working on data and research projects. Some of them, like this, actually get published here, others ... not so much. This work tends to eat up a fair amount of time that I could be spending biking.

I'm also in a relationship; shout-out to Emma, who will be serving as the bookkeeper for this whole thing and helped workshop all of these ideas. We spend a good deal of time together during the weekday evenings and weekends, which I would rather do than being on a bike for hours.

I have a few vacations planned for this spring/summer, which will limit my ability to ride. On the other hand, spring and summer is the most pleasant time to ride, so I will most likely be logging more hours per weekend on average. 
