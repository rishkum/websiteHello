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

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/democracies_Weak.png)
Are democracies slow?

Using data from The Economist and the John Hopkins, the outlook for democracies do look a bit grim. There is a pretty positive relationship with the level of democracy one country is and the number of corona cases that country has.  



What could be the reason for this? Perhaps it's just that democracies were slow at responding. But then looking at the data does not really look like that.:

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/lockdown_implementation.png)


__Does the response even matter?__

Using data from The Economist and the John Hopkins, the outlook for democracies do look a bit grim. There is a pretty positive relationship with the level of democracy one country is and the number of corona cases that country has.  


What could be the reason for this? Perhaps it's just that democracies were slow at responding. But then looking at  the data does not really look like that.:

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/loackdown_effects.png)


__Let's do some analysis. . Smaller model to bigger__
Economist use regressions to predict how one or multiple factors can affect something. Because in life multiple things affect one thing, its difficult to pin-point at what leads to what and what is the major reason behind some event. 

![](/post/2020-05-11-democracies-in-the-time-of-covid_files/regression_outputs.png)


In the case of Corona virus cases, I created a set of models to understand how different factors affect the level of corona virus cases a country has. More information about the dataset and the analysis can be found on my Github. 


__What it all means__
If you are only considering the effect of level of democracy to the level of cases then you do see some relationships among that. However when you start up adding other factors such as average age, average temperature, Gap, per-capita things start to change. 



Correlation is not causation[^1]


[^1]:dhghfhgfh


