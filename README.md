# README

# How to run Natours Starter website (What I wrote)

```
cd Natours/starter/
npm run compile:sass // compile sass
live-server // Get hot reload - make sure live-server is installed globally
```

I was a fan of these slides:

![image](./Natours/starter/img/slide_1.png)

![image](./Natours/starter/img/slide_2.png)

We also want to use em and rem. This is because it gives us an easy way to scale lengths along with font-size (see pic below).

em == "emphemeral unit"- see below for what it means in practice.
em vs rem - rem is relative to root font-size.

```
Note: Below image is a bit confiusing because you need to match the numbers (x) to the css. But the math does work.
```

![image](./Natours/starter/img/slide_3.png)
![image](./Natours/starter/img/slide_4.png)

Inheritence:

![image](./Natours/starter/img/slide_5.png)
![image](./Natours/starter/img/slide_6.png)

# How a website renders once css has been resvoled and process.

The visual formatting model:

![image](./Natours/starter/img/slide_a0.png)
![image](./Natours/starter/img/slide_a1.png)
![image](./Natours/starter/img/slide_a2.png)
![image](./Natours/starter/img/slide_a3.png)
![image](./Natours/starter/img/slide_a4.png)
![image](./Natours/starter/img/slide_a5.png)
![image](./Natours/starter/img/slide_a6.png)

# Advanced CSS and SASS

These are the main responsive design _TECHNIQUES_:
Fluid layouts - really just a practice of writing css in a scalable manner.

![image](./Natours/starter/img/adv_1.png)

Layout types when thinking about fluid layouts (these are supported by all browsers):

Note: Float layouts are kind of old and getting replaced by flexbox and css grid (flex and grid have revolutionized css).

![image](./Natours/starter/img/adv_2.png)
![image](./Natours/starter/img/adv_3.png)
![image](./Natours/starter/img/adv_4.png)
![image](./Natours/starter/img/adv_5.png)
![image](./Natours/starter/img/adv_6.png)
