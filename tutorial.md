# tutorial

## Step 1 - Get set up

Remove the  ``||basic:start||``   and  ``||basic:forever||``  blocks and bring in an ``||input:onButtonPressed||`` block. It can be set to "A" or "B" for the block that is the trigger.
    
```ghost
input.onButtonPressed(Button.A, function () {
    
})
```

## Step 2 - Bring in a repeat

Insert a ``||loops:repeat||`` inside of the ``||input:onButtonPressed||`` block. Change the number of repeats to 40.

```blocks
input.onButtonPressed(Button.A, function () {
    for (let index = 0; index < 40; index++) {
        
    }
})
```

## Step 3 - Insert the tone block

Grab a ``||music:play tone||`` block and place it inside of the ``||loops:repeat||`` block.

```blocks
input.onButtonPressed(Button.A, function () {
    for (let index = 0; index < 40; index++) {
        music.playTone(262, music.beat(BeatFraction.Eighth))
    }
})
```

## Step 4 - Add some Randomness!

Now let's add some Randomness by putting in a ``||math:random||`` block into the ``||music:play tone||`` block. Change the upper and lower values to 988 and 131. Double check that the beat is set to 1/8.

```blocks
input.onButtonPressed(Button.A, function () {
    for (let index = 0; index < 40; index++) {
        music.playTone(randint(131, 988), music.beat(BeatFraction.Eighth))
    }
})
```

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>