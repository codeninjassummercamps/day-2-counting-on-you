# Day 2 Counting On You

## Counting On You

In this activity, you will show what you've learned about variables by making a custom counter.

## Step 1

The first thing you will need to do is to create a variable to be a counter. Then, set it to 0 when the code starts.

```blocks
let count = 0;
```

## Step 2

Create an ``||player.on chat command||`` that will display the value of the counter using a ``||player.say||`` block. You can drag any ``||variables||`` you make into say blocks to show their value!

```blocks
let count = 0;
player.onChat("counter", function () {
    player.say(count)
})
```

## Step 3

Several different events are available for you in this activity! Select an event that you like, and when that event occurs, ``||variables.change||`` the count! (An example is provided in the hint.)

```blocks
let count = 0;
mobs.onMobKilled(SHEEP, function(){
    count += 1;
})
```

## Step 4

Pick at least 2 more events, and add code to change the counter in each. Don't forget you can use a negative number to decrease the counter!


## Step 5

Go ahead and try out your code and make sure everything is working. If it's not, look back at the hint on step  3 or ask a Sensei!

## Step 6

Is all your code working? The hint has some examples of events you could have created!

```blocks
let count = 0;
mobs.onMobKilled(SHEEP, function(){
    count += 1;
})
player.onTravelled(TravelMethod.walk, function(){
    count += 2;
})
player.onDied(function(){
    count += -10;
})
player.onItemInteracted(DIAMOND_SWORD, function(){
    count += 3;
})
blocks.onBlockPlaced(GRASS, function(){
    count += 5;
})
blocks.onBlockBroken(GRASS, function(){
    count += -5;
})
player.onArrowShot(function(){
    count += 100;
})
```

## Bonus!

Can you figure out how to make an ``||player.on chat command||`` that will reset the counter back to 0?

```blocks
player.onChat("reset", function(){
    count = 0;
})
```

## Activity Complete!

You did it! You showed off what you know about variables (and events)!
