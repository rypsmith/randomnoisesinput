# tutorial

## Step 1 - Get set up

Remove the  ``||basic:start||``   and  ``||basic:forever||``  blocks and bring in an ``||input:onButtonPressed||`` block.
    
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

