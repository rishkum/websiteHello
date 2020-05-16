---
title: Democracies in the time of Covid
author: Rishabh Kumar
date: '2020-05-11'
slug: democracies-in-the-time-of-covid
categories:
  - data visualisation
  - covid
tags:
  - coronavirus
  - covid19
  - data visualisation
  - regression
toc: no
images: ~
enableEmoji: true
comments: true
---
Over the past weeks I have had conversation with families and friends about coronavirus and about how different governments are responding to the challenge. One point that was mentioned often in the discussion was that its the countries with stronger government that have stayed off the crisis whereas democratic countries are the ones who cannot fight off the pandemic. Just because democracies make it slow.

I live in a democracy and believe in democracies :two_hearts: so I did find this idea a bit off-putting. But then arguing an argument with blanket statement isn’t the best things to do. To find the real story, one has to dig in and figure out what is actually happening. Even though data is still coming across here, we still have some interesting stats to make an evidenced based guess about what is happening.

**On the first look:**

Using data from The Economist and the John Hopkins, the outlook for democracies do look a bit grim. There is a pretty positive relationship with the level of democracy one country is and the number of corona cases that country has.  What could be the reason for this?

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/democracies_Weak.png)

**Are democracies slow?**

```{r, eval=T}
par(mar = c(4, 4, .1, .1))
plot(pressure, pch = 19, type = 'b')
```

knitr:: include_graphics('post/2020-05-11-democracies-in-the-time-of-covid_files/lockdown_implementation.png')


Perhaps it's just that democracies were slow at responding to the crisis. Looking at the data it does not really look like that. There were some fully democratic countries who took their in imposing lockdown  after observing the first case of coronavirus.

Nonetheless, there is not a  statistically significant relationship between the level of democracy in a country and the swiftness of strict response. One possible reason for this could be all countries were in the hope that this virus would miraculously vanish. Imposing lockdown is expensive and perhaps countries wanted to avoid these costs.



__Does the response even matter?__

This an important question. If countries were imposing lockdown would their cases been lower. It turns out there is a positive relationship among number of days a country takes to imposing lockdown and the total cases per million present in that country.

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/loackdown_effects.png)


__Let's do some analysis...__

Economists use regressions to predict how one or multiple factors can affect something. Because in life multiple things affect one thing, its difficult to pin-point at what leads to what and what is the major reason behind some event. Multivariate regressions, here help us  control for effect of different variables and then help us isolate their net impact on the variable of interest. 

The following graph shows two models, one where I am using just the democracy index to predict the no of cases in a country and the second model shows where I am using other variables to predict the number of Covid-19 cases in a particular country. 

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/regression_outputs.png)


__What it all means__
If you are only considering the effect of level of democracy to the level of cases then you do see some relationships among that. However when you start up adding other factors such as average age, average temperature, Gap, per-capita things start to change. 

The analysis shows that if a country is democratic and has an older population only then it would show increases in the number of cover cases. On itself a democracy does not increase the level of covid cases in a country.


Media often narrowly focuses on a particular case and then declares it as a norm. It's crucial that we think about these statements critically and then put our belief in them. 



