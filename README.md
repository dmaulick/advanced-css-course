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

# Flexbox Lessons

Codepen to mess around: https://codepen.io/dmaul08/pen/XWeYqMN

This is a good video to watch with for container: https://www.udemy.com/course/advanced-css-and-sass/learn/lecture/8274576#overview

This is a good video to watch with for items: https://www.udemy.com/course/advanced-css-and-sass/learn/lecture/8274580#overview

**Container**

flex-direction - direction of main axis

flex-wrap - what happens when not enough space in container

justify-content - how flex items are aligned on main axis

align-items - how flex items will align on cross axis. (often used in combo justify-content). This is easiest to reason about (assuming flex-direction: row) when the items are different heights. align-item: center will align other items in middle of largest item/ align-item puts small items at bottom/ stretch, stretches all smaller items to be height of largest. Special one: align-item: baseline will align their items along their common text.

align-content - only applies when more than one row of flex items. When case is possible this controls how the rows are spaced across cross axis. default value: align-content: normal which packs lines in normal position as if this was never set.

**Item**

align-self - similar to align items but applies only to specific item

order - specify where one specific item should appear in order with other items. By default items have order: 0. So if you put -1 it will override that one to be at start, or 1 will put at the end.

The following help flexbox decide on the width of a flex item:

flex-grow - how much can grow. Remember these are relative to other items in flex container. So by default all items have flex-grow: 0, so if just one then has flex-grow: 1 it will take up as much room as possible. Another cool case: if all have flex-grow: 1 and a single item has flex-grow: 2 the latter will be twice the size of all others.

flex-shrink - controls how much an item can shrink. Flex-shrink has the initial value flex-shrink: 1 which allows shrinking. If set flex-shrink: 0 they will no longer shrink.

flex-basis - base width. We use this to set flex items instead of width property. Intial value is flex-basis: auto. But will commonly override to a percentage that will set its width to a percentage of the container (can still set a px but perc is better).
flex - (ex: flex: 0 1 auto (\<int> \<int> \<len>)) - short hand for flex-grow flex-shrink flex-basis

![image](./Nexter/starter/img/flex_1.png)

# CSS Grid Lessons

Note: Firefox has best grid dev tools.

Codepen set up for practicing: https://codepen.io/dmaul08/pen/BawVVLj

![image](./Nexter/starter/img/grid_0_1.png)
![image](./Nexter/starter/img/grid_0_2.png)
![image](./Nexter/starter/img/grid_1.png)

Screenshot of codepen that should trigger some memories of hwo to work with grid.
![image](./Nexter/starter/img/grid_2.png)
