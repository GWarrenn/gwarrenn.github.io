---
layout: post
title: Sport or Not!
---

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/Sports%20Header.png)

About The Survey
--------------

Following up in the [rich tradition](https://gwarrenn.github.io/Fruit-Ranking/) of creating surveys that throw a Molotov cocktail into any social situation, I presented another question to the world/my small network of people with opinions: <b>Are these things sports?</b>

While the [sports literati](https://bleacherreport.com/articles/848465-settling-the-debates-is-it-a-sport-or-not-a-sport) sit in their ivory towers and get to decree whether or not certain things are sports or not, I give the power to the people to decide! Respondents were presented with a list of 19 activities that are borderline sports and could or not be considered a sport depending on who you ask. The activities ranged from Skiing to Frisbee Golf to Scrabble (In order to avoid bombarding respondents with a battery of 50 items, I excluded things that are considered mainstreams sports). The survey also asked respondents how they define sports in an effort to help understand what makes a sport a sport.

Miss out on the survey? Here's a [link to the survey](https://forms.gle/LGXMaLbPw3ahA2Ef6), which is still open, and you can help contribute to further work by [adding your opinion here!](https://docs.google.com/forms/d/e/1FAIpQLSeH8yw7-P18_G3hqGqvK7eMEtN20xg1rkkQBY89eAeJDGgrfw/viewform) 

<details>
<summary>See How Your Perceptions of Sports Align With the Field</summary>
<br>
<figure class="video_container">
<iframe width="800" height="600" src="https://raw.githack.com/GWarrenn/this-and-that/drafting/sport-or-not!/scripts/comparison/index.html" frameborder="0" allowfullscreen="true"></iframe>
</figure>
</details>

Overall Perceptions of Sports
--------------

On average, the field is adamant that Rowing/Crew is the most of a "Sport" of all activities tested -- even though it's basically just going for a canoe ride with a dozen people and yet Chess, a sport that requires skill and training and [tons of physical endurance](https://www.espn.com/espn/story/_/id/27593253/why-grandmasters-magnus-carlsen-fabiano-caruana-lose-weight-playing-chess) <b>IS NOT SPORT WELL OKAY THEN FINE</b> -- with nearly three quarters stating they feel strongly it's a sport. NASCAR is really the only activity than comes close to being net even on the Sport/Not Sport divide, with 55% for to 42% against. 

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/2.0%20Ratings%20by%20Sport.png)

Most of the "indoor" or leisure activities (Crossfit, eSports, Foosball, Chess, and Scrabble) were solidly designated as "Not Sports," with the strongest intensity coming for Scrabble. Another item of note, approximately half the respondents had no idea what Pickleball is, including myself. If you want someone to blame, contact [Ben Winston](https://www.strategies360.com/team/ben-winston/) for an explanation or any general research inquiries (#ad #promotion). 

Relationships between Activities
--------------

The following chart shows the correlations, or similarities, between each of the activities tested - a score of 1 indicates that everyone picked exactly the same thing, while a score of -1 indicates the opposite. Some strong positive relationships can be found between the activities that were definitely selected as sports, such as Skiing, Rowing/Crew, and Cycling. However, the strongest negative relationships are found between Snowboarding and Scrabble, meaning that if you thought Snowboarding was a sport, then you probably don't think Scrabble is a sport (and vice verse). 

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/3.0%20Correlation%20Matrix.png)

Perceptions by Gender
--------------

Overall, women are more skeptical that the activities tested are actually sports; women tended to rate 52% of the activities as sports compared to 64% among men. Views tend to align on the more commonly accepted sports, such as Cycling and Skiing. However things tend to break down among the more contentious activities, specifically NASCAR. Only 29% of women view NASCAR as a sport, compared to 65% of men. Bowling, Frisbee Golf, Cornhole, and eSports are also viewed differently by gender. Controlling for race, income, sports fandom (more on that later) and age, men are are 3.38 times more likely than women to view NASCAR as a sport -- this is the largest coefficient observed in this dataset, second only to eSports at 2.65 times more likely. ![(Full regression results here)](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/Regression%20Coefs.png)
    
![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20Gender.png)

Before we look at other demographics tested, we should also talk about views towards sports in general by gender. The survey also asked sports watching behaviors and favorability towards PE/Gym class, which turned out to be influenced by gender, so we need to examine the relationship before we talk about the other demographics by themselves.

Views towards PE/Gym class by gender are nearly a mirror image. Just under half of women who took the survey were strongly unfavorable towards P.E./Gym class when they were in school, compared to only 5.6% of men. Overall men were net favorable towards PE, while women were strongly net unfavorable towards PE. At first glance it might be a reflex to chalk this difference entirely up to gender. However, the survey also asked two questions that allowed respondents to state if they were avid/casual sports fans or not at all and how often they watched televised sports. These two variables were combined to create a "Sports Fan" variable[¹](#sports-fan-def)(credit to Ben Winston & Kelly Higgins for their input in creating this). 

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/Sports%20%26%20Gender.png)

When we include this Sports Fan variable in a binomial regression model that predicts favorability towards PE/Gym class, along with Gender, the Sports Fan variable is the stronger predictor of favorability. Gender is still highly predictive, but the correlation and regression coefficient is lower than Sports Fandom.

<table style="text-align:center"><tr><td colspan="2" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"></td><td><em>Dependent variable:</em></td></tr>
	<tr><td></td><td colspan="1" style="border-bottom: 1px solid black"></td></tr>
	<tr><td style="text-align:left"></td><td>Gym Class Favorability</td></tr>
	<tr><td colspan="2" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left">Gender (Men=1)</td><td>1.118<sup>***</sup></td></tr>
	<tr><td style="text-align:left"></td><td>(0.430)</td></tr>
	<tr><td style="text-align:left"></td><td></td></tr>
	<tr><td style="text-align:left">Sports Fandom (Sports Fan=1)</td><td>1.401<sup>***</sup></td></tr>
	<tr><td style="text-align:left"></td><td>(0.429)</td></tr>
	<tr><td style="text-align:left"></td><td></td></tr>
	<tr><td style="text-align:left">Constant</td><td>-1.346<sup>***</sup></td></tr>
	<tr><td style="text-align:left"></td><td>(0.345)</td></tr>
	<tr><td style="text-align:left"></td><td></td></tr>
	<tr><td colspan="2" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left">Observations</td><td>113</td></tr>
	<tr><td style="text-align:left">Log Likelihood</td><td>-61.558</td></tr>
	<tr><td style="text-align:left">Akaike Inf. Crit.</td><td>129.117</td></tr>
	<tr><td colspan="2" style="border-bottom: 1px solid black"></td></tr><tr><td style="text-align:left"><em>Note:</em></td><td style="text-align:right"><sup>*</sup>p<0.1; <sup>**</sup>p<0.05; <sup>***</sup>p<0.01</td></tr>
</table>

With a regression coefficient of 1.15, men are <b>3 times more likely</b> than women to be favorable toward PE/Gym Class. However, Sports Fandom has a coefficient of 1.4 (meaning <b>4 times more likely</b> than non-Sports Fans to be favorable towards PE/Gym Class). <b>So this means that women who are Sports Fans are more likely to be favorable towards Gym class than men who are not Sports Fans at all.</b>

Perceptions by Race/Ethnicity
--------------

<i>Just a note on how race is reported herein: Because the overall N-size of the survey is only just over 100, I combined certain racial groups into "POC" as each individual POC racial group was less than 10. (POC N=24 & White N=89, with the POC portion skewing male and white portion skewing female.</i> 

On average, POC respondents were less bullish on Rowing/Crew, Ultimate Frisbee, Snowboarding, and Skiing than White respondents, though they resoundingly still classified them as sports. Interesting differences are observed with NASCAR (which is most likely driven by the more male skewed POC sample), Frisbee Golf, and Chess. White and POC respondents are flipped on both NASCAR and Frisbee Golf, and only 12% of White respondents agreed that Chess is a sport (with 65% stating it is strongly not a sport), compared to a third POC respondents.

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20Race.png)

Perceptions by Age
--------------

Intensity towards the belief that cycling is strongly a sport seems to increase by age; 92% of respondents over the age of 40 felt strongly that cycling is a sport. Similarly, older respondents were much more united around sailing and Pickleball being sports and eSports not being sports, with more higher intensity than younger respondents. 

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20Age.png)

Perceptions by Other Demographics
--------------
___

<details>
<summary>Perceptions by Income</summary>
<br>
<img align="middle" src="https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20Income.png"/>
</details>

___

___

<details>
<summary>Perceptions by PE/Gym Favorability</summary>
<br>
<img align="middle" src="https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20PE%20Therm.png"/>
</details>

___

What Defines a Sport?
--------------

In addition to classifying activities as sports, respondents were also asked to write what defines a sport in their opinion in an open-ended format. Overall, the most commonly used word (excluding and filler words) was 'physical' mentioned 52 times, followed by 'competition' and 'activity' mentioned 39 and 25 times, respectively. Reflecting the emphasis on the required physical nature of the sport, the most commonly used pair of words (or bigrams) were 'physical activity','physical exertion', and 'physical skill'. Given this, it makes sense just why our "indoor sports" and leisure sports failed to pass judgment as sports. 

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/N-Grams.png)

Naturally, the more cerebral or strategic activities, such as eSports, Chess, and Scrabble are more perceived moreso as a sports among respondents who did not mention the word "physical" in their definition of a sport, though the activities were still resoundingly classified as not sports by both groups. Respondents who did not mention physical actually perceive NASCAR to be less of a sport than those who mentioned physical. Additionally, the "Non-Physical" camp is much more intense in their belief that sailing is strongly considered a sport.

![](https://raw.githubusercontent.com/GWarrenn/this-and-that/drafting/sport-or-not!/images/4.0%20Sport%20Ratings%20by%20Mentioned%20Physical.png)

Further Work
--------------

If the 113 people are the ones to judge, there is a clear need for a certain amount of physicality or physical exertion, however the same group also determined that Crossfit is very much not a sport. These same people also described a certain amount of skill or strategy required, but less so that the physical element. Is there a hard or definable threshold of perceived physical exertion that makes something a sport along with a combination of a certain amount of skill and/or competition? Can that nexus of physicality, skill and competition be quantified and modeled or is the definition of a sport something that is arbitrary and hypocritical?

<b>[YOU DECIDE](https://docs.google.com/forms/d/e/1FAIpQLSeH8yw7-P18_G3hqGqvK7eMEtN20xg1rkkQBY89eAeJDGgrfw/viewform)</b>

Take the survey linked above and help us try to build a definitive taxonomy of sports. 

Conclusion
--------------

If I've done my job (I should really get back to work) then you will have found something appallingly wrong or antithetical to your world view here -- video games are sports, I don't care what 77% of you think!

Thank you to everyone who took this survey and/or shared it with others. I sincerely appreciate you all taking the time to take these surveys and read (\*skim) these posts. I look forward to arguing with everyone about this in person.

Footnotes
--------------
^[1.](#sports-fan-def)"Sports Fans" are defined as respondents who self-identify as avid or casual mainstream sports fans who also claim to watch televised mainstream sports at least once a week. This segment came out to be about half of the sample.