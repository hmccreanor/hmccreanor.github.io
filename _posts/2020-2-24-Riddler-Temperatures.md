---
layout: post
title: Riddler Express - Farenheit to Celsius
---

{% include mathjax.html %}

The Riddler Express puzzle for this week involves finding temperatures that, when converted from Farenheit to Celsius, are mirror images of each other i.e: $$61 \degree F$$ and $$16 \degree C$$.
A more complete explanation can be found [here](https://fivethirtyeight.com/features/can-you-flip-your-way-to-victory/).

In essence, we are looking for solutions to the following equation:

$$
f = \frac{9}{5}c + 32
$$

where $$f = 10a + b$$ and $$c = 10b + a$$ with $$a$$ and $$b$$ representing the digits of the temperatures (I assumed that the temperature was going to be two digits long). 

This leads to the equation:

$$
a = \frac{160 + 85b}{41}
$$

As $$b$$ is just an integer from $$0$$ to $$9$$, then we can just substitute in various values for $$b$$ until we get an $$a$$ value that is approximately equal to an integer in this range.

Indeed, we see that when $$b = 1$$, $$a \approx 6$$, and when $$b = 2$$, $$a \approx 8$$. We are told that the temperature is not $$61 \degree F$$ and so consequently it is $$82 \degree F$$.
