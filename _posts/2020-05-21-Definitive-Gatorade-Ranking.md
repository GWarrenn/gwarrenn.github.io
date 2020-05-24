---
layout: post
title: Definitive Gatorade Ranking
---

About The Survey
--------------

Like many people living in quarantine during the current pandemic, I've found myself engaging in deep, heartfelt conversations with those who are forced to live with me. One such ~~argument~~ conversation started after one of my roommates broke the deafening silence that had been haunting the house as we've run out of things to talk about when they noticed a Gatorade in the room and thought "yes, this is the thing that we will talk about now." Now, I consider myself a Gatorade connoisseur, having imbibed the sweet, sweet juice throughout my youth to this day, and thought that I had a pretty refined taste. However, I quickly learned that **some** of my roommates think that Orange Gatorade is trash, while the other half (the enlightened half) think that Orange Gatorade is good. This news was a revelation: _how could someone not agree with me on Gatorade?_

To help answer this question, I turned to the only tool at my disposal: a survey of a non-random sample of people that is nowhere near representative of the general public. So, to the Gatorade marketing team reading this, take the findings with a grain of salt, but also maybe throw some Gatorade swag my way?

The survey is still open and collecting responses, but as of publishing this, 398 people have thrown their takes into the crucible of public opinion. So, if you haven't taken it yet, please go here: [](https://forms.gle/DYo7zotAp7BTZc1T6) and fill the survey out before reading on.

Definitive Gatorade Ranking
--------------

Overall, the two blue Gatorades top the charts of public opinion, with Icy Charge from the Frost series narrowly leading Cool Blue. The two more classic offerings, Lemon Lime and Fruit Punch, come in at third and fourth place. 

Funnily enough, attitudes towards Orange Gatorade nearly matches my household consensus; half of respondents ranked Orange as A/B-tier, while the other half ranked it in the C/D/F-tiers. 

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/1_overall_ratings.png)

Similar to the Fruit Survey, I created a Gatorade GPA, which converts the grade ranking to a 0-4.0 GPA scale, which allows for a single data point that captures the distribution of rankings and removes any "Never tried" responses from the equation.  

Even when we remove the "Never tried" responses, the more rare offerings, such as Green Apple, Lime Cucumber, and Strawberry Watermelon, still score the lowest. Strawberry Lemonade stands out as one of the underappreciated gems; a third of respondents had never tried it, but those who have tried it rate it higher than average. 

Additionally, both of my personal favorites -- Fierce Grape and Orange -- are in the Square of Death, with higher than average familiarity and lower than average ranking. If you need to reach me, I'm going to be in a dark room coping with the fact that I have poor taste in Gatorade.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/1_1_name_recognition_plot.png)

_Everything to the left of the vertical line above are rated lower than average and everything to the right is rated higher than average. Similarly, everything below the line is less well know/tried than average and everything above is more well known/tried._

Unsurprisingly, there are similarities in preferences between certain flavors. The strongest correlations in preferences can be found with the two Strawberry flavors tested -- Strawberry Lemonade and Strawberry Watermelon. Additionally positive relationships can be found two of the three Frost flavors tested -- Icy Charge and Arctic Blitz.

On the other hand, the strongest negative relationships can be found with Lime Cucumber and Fruit Punch -- we'll get into the driving forces behind this later on.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/2_correlations_matrix.png)

Gatorade Ranking by Demographics
--------------

As always, topline numbers are great, but what we really want to see is how the numbers change within and compare across various demographic groups.

### Opinions by Gender

On average, men rated all of the colors slightly higher than women and non-binary respondents. Generally, attitudes across the gender spectrum tend to follow the same overall pattern, though with a varying degrees of intensity. However, interesting differences in taste preference can be found with Grape/Purple and Strawberry Lemonade.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/3_1_demo_gender_recode_plot.png)

While men may have a higher average Gatorade GPA, women have a much wider distribution of opinions -- which can be found in the higher rating of Icy Charge and a much lower rating of Green Apple. Men tend to cluster closer to the mean score, while women show greater variety of opinions.  This backs up [previous research](https://gwarrenn.github.io/Fruit-Ranking/) on fruit preference, which showed a similar distribution of opinions by gender.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/4_distribution_gender_plot.png)

### Opinions by Ideology

Politics are becoming more and more inescapable; creeping into [conversations around sports](https://www.pbs.org/newshour/politics/in-the-trump-era-separating-sports-and-politics-is-harder-than-it-seems) and [whether or not you listen to your doctor](https://www.cnn.com/2020/04/20/politics/stay-at-home-protests-conservative-groups-support/index.html), but does ideological identity also impact Gatorade preference? No, not really, though that would be a cool headline if it did, wouldn't it?

Our (very small) group of Conservative/Libertarian respondents are the most favorable towards Gatorade overall, showing the strongest support for the Lemon Lime -- the most traditional of all Gatorade flavors. 

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/3_5_demo_ideo_recode_plot.png)

### Opinions by Age

Of all of the demographics tested, age proved to demonstrate the greatest gulfs in opinion. Survey respondents over the age of 40 viewed the more "traditional" flavors, such as Fruit Punch and Orange most favorably and more favorably than younger respondents, and showed strong distaste for Lime Cucumber (remember the negative correlation between Fruit Punch and Lime Cucumber from before?). On the other hand, the respondents in the youngest age bracket (18-29) are much more favorable to "the blues" -- Icy Charge, Electric Blue and Arctic Blitz.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/3_2_demo_age_recode_plot.png)

Further illustrating the significant role that age plays in attitudes towards Gatorade preference, I ran a series of logistic regression models to predict positive attitudes towards each flavor tested. Across all of the flavors where we saw a generational divide, age was the only significant predictor of preference when controlling for race, gender, income and favorability towards Gatorade. Also of note, men were more likely to be favorable towards Grape and Lemon Lime than women.

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/5_Regression Coefs.png)

To bring this all together (and because I could), I ran a Principal Component Analysis to further illustrate the grouping of the various flavors and attitudes by demographics. This helps map out clusters of similar flavors: we can see a grouping of our more popular flavors, including the Blues and Lemon-Lime. However, Fruit Punch, while being a popular choice is off in it's own segment with our 40+ survey respondents. 

Lime Cucumber, unknown and unloved to most, is off in its own part of the graph plotting our demise.  

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/PCA.png)

Flavor or Color: How do you refer to Gatorade?
--------------

As you've probably noticed, I've been referring to each of the Gatorade types interchangeably as both flavors and colors. I do this mostly because there are four or five "blues" and a few yellows, but in general if someone is going to the store asks if I want anything, I won't say "get me some of that Riptide Rush." Instead, I'll just say "purple," knowing full well that there are many options but I'll generally be happy with anything in that part of the color spectrum. 

However, there are some out there who don't use this technique -- despite the fact that it's [pretty well established](https://www.google.com/search?q=calling+a+gatorade+by+its+flavor+meme&safe=off&rlz=1C1GCEV_en&sxsrf=ALeKk02Q_dlfDYw4VApkam3RTJJ7ydD4Qw:1590095261870&source=lnms&tbm=isch&sa=X&ved=2ahUKEwjljvi57sXpAhWzknIEHdHrAjMQ_AUoAXoECAsQAw&biw=1280&bih=610) that you can't trust people who refer to Gatorade by the flavor -- so I decided to include this as a demographic question.

Overall, our survey respondents overwhelmingly report that they refer to a specific Gatorade by the color, not the flavor -- with 85% against 15%. This pattern (mostly) holds true across all demographics, with the majority reporting that they refer to the color. However, nearly a third of our (admittedly, very small N-size) Conservative/Libertarian respondents use the flavor as a descriptor. 

![](https://raw.githubusercontent.com/GWarrenn/gwarrenn.github.io/gatorade-ranking/images/gatorade_ranking/6_Flavor or Color -- Demos.png)

Of course, as with all things in this survey, age is yet again the only significant predictor on this topic. When controlling for age, Gatorade favorability, gender, ideology, income, and race, younger respondents are more likely to refer to Gatorade by the color (and the inverse is true for older respondents).

Thanks & Conclusion
--------------

Thank you to everyone who took the survey and eagerly shared it with their network -- special thanks to my roommates Mahkah, Mika and Chris (even though some of them are wrong about Orange Gatorade) for pushing me to actually release the survey after I wrote it and then was too chicken to send it out and [the Snacket](https://www.facebook.com/groups/391870207855543/) for just being crazy fanatic about snacks. Obviously I wouldn't be able to do any of this work without you all taking the time to enter your opinions.  


Survey Demographics
--------------

<a name="footnote-demo-table"></a>
<html>
<meta http-equiv="Content-type" content="text/html; charset=UTF-8">

<head>
<div style="margin: 0 auto; display: table; margin-top: 1em;">
<table class="gmisc_table" style="border-collapse: collapse; margin-top: 1em; margin-bottom: 1em;" id="">
<thead>
<tr><td colspan="4" style="text-align: left;">
Demographic Summary Table</td></tr>
<tr>
<th style="font-weight: 900; border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;"></th>
<th style="border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;">Response</th>
<th style="border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;">N</th>
<th style="border-bottom: 1px solid grey; border-top: 2px solid grey; text-align: center;">Percent</th>
</tr>
</thead>
<tbody> 
<tr><td colspan="4" style="font-weight: 900;">Age</td></tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">18-29</td>
<td style="text-align: center;">199</td>
<td style="text-align: center;">51.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">30-39</td>
<td style="text-align: center;">168</td>
<td style="text-align: center;">43.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">40+</td>
<td style="text-align: center;">27</td>
<td style="text-align: center;">7.0%</td>
</tr> 
<tr><td colspan="4" style="font-weight: 900;">Income</td></tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Under $50,000</td>
<td style="text-align: center;">80</td>
<td style="text-align: center;">20.0%</td>
</tr> 
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">$50,000 to $100,000</td>
<td style="text-align: center;">141</td>
<td style="text-align: center;">36.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Over $100,000</td>
<td style="text-align: center;">112</td>
<td style="text-align: center;">28.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Prefer not to disclose</td>
<td style="text-align: center;">61</td>
<td style="text-align: center;">15.0%</td>
</tr>
<tr><td colspan="4" style="font-weight: 900;">Ideology</td></tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Conservative/Libertarian</td>
<td style="text-align: center;">16</td>
<td style="text-align: center;">4.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Leftist</td>
<td style="text-align: center;">93</td>
<td style="text-align: center;">24.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Liberal</td>
<td style="text-align: center;">202</td>
<td style="text-align: center;">51.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Moderate</td>
<td style="text-align: center;">43</td>
<td style="text-align: center;">11.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Prefer not to disclose</td>
<td style="text-align: center;">40</td>
<td style="text-align: center;">10.0%</td>
</tr> 
<tr><td colspan="4" style="font-weight: 900;">Gender</td></tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Female</td>
<td style="text-align: center;">211</td>
<td style="text-align: center;">54.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Male</td>
<td style="text-align: center;">161</td>
<td style="text-align: center;">41.0%</td>
</tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">Other</td>
<td style="text-align: center;">22</td>
<td style="text-align: center;">6.0%</td>
</tr> 
<tr><td colspan="4" style="font-weight: 900;">Race/Ethnicity</td></tr>
<tr>
<td style="text-align: left;">&nbsp;&nbsp;	</td>
<td style="text-align: center;">POC</td>
<td style="text-align: center;">67</td>
<td style="text-align: center;">17.0%</td>
</tr>
<tr>
<td style="border-bottom: 2px solid grey; text-align: left;">&nbsp;&nbsp;	</td>
<td style="border-bottom: 2px solid grey; text-align: center;">White</td>
<td style="border-bottom: 2px solid grey; text-align: center;">327</td>
<td style="border-bottom: 2px solid grey; text-align: center;">83.0%</td>
</tr>
</tbody>
</table>
</div>
</body>
</html>
