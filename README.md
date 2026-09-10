# Fantastic Creatures Incorporated

### @explicitHints true

## Welcome, ranger!

Hello ranger! Welcome to your first day on the job at Fantastic Creatures Incorporated! We plan on placing 3 animals into your care today.

Each animal needs food, water, and love.

To keep track of all the different things each animal needs, we will need ``||variables(noclick):Variables||``.

``||variables(noclick):Variables||`` are simply **containers that we can store values inside**. ``||variables(noclick):Variables||`` can hold anything, and today you will store numbers, words, and lists in them as you take care of your animals.

``||variables(noclick):Variables||`` can be ``||variables(noclick):set||`` (where we *erase* what was inside before and *replace* it) or ``||variables(noclick):changed||`` (where we *add* or *remove* something from the ``||variables(noclick):variable||`` but leave the rest alone).

To start let's update the ``||variables(noclick):variable||`` for your 1st creature!

## 1. Bring in Dragon

Your 1st enclosure is ready for Dragon. The game needs somewhere to keep that choice.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your 1st creature.**

### Add this code

- [ ] Open ``||variables(noclick):Variables||``.

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):animal1||``.

- [ ] From ``||loops(noclick):Loops||``, drag an ``||loops(noclick):on start||`` block into the workspace.

- [ ] From ``||variables(noclick):Variables||``, place ``||variables(noclick):set animal1 to||`` inside ``||loops(noclick):on start||``.

- [ ] Open **Advanced** → ``||text(noclick):Text||``.

- [ ] Put the ``||text(noclick):" "||`` word block into ``||variables(noclick):set animal1 to||``.

- [ ] Type ``||text(noclick):Dragon||`` between its quotes.

- [ ] From ``||animalCare(noclick):Care Displays||``, add ``||animalCare(noclick):show value in the 1st enclosure||`` under the ``||variables(noclick):set||`` block.

- [ ] Put ``||variables(noclick):animal1||`` into that show block.

### What you should see

- [ ] Run your game.

- [ ] Click the game screen.

- [ ] Use the arrow keys to walk around.

Your Dragon should appear in the 1st enclosure.

**Keyboard controls:** **Space** is the **A** button. **Enter** is the **B** button.

![first arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/01-first-arrival.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let animal1 = ""

animal1 = "Dragon"

animalCare.showAnimal1(animal1)
```

## 2. Name Dragon

Your Dragon needs a name.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Dragon's name.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):dragonName||``.

- [ ] Pick one name: `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] In ``||loops(noclick):on start||``, place ``||variables(noclick):set dragonName to||`` under the block that shows ``||variables(noclick):animal1||`` in the 1st enclosure.

- [ ] Put the ``||text(noclick):" "||`` word block from **Advanced** → ``||text(noclick):Text||`` into the ``||variables(noclick):set||`` block.

- [ ] Type the name you chose between its quotes.

- [ ] From ``||animalCare(noclick):Care Displays||``, add ``||animalCare(noclick):show value beside Dragon||`` under the ``||variables(noclick):set||`` block.

- [ ] Put ``||variables(noclick):dragonName||`` into that show block.

### What you should see

- [ ] Run your game.

A wooden name sign should keep showing your chosen word on the front-right fence of Dragon's enclosure. A message at the top should briefly welcome Dragon by that name.

![first name: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/02-first-name.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let dragonName = ""

dragonName = "Pip"

animalCare.showDragonName(dragonName)
```

## 3. Give Dragon love

Your Dragon's heart meter is empty. Pet your creature with empty hands so its love can change.

The supplied ``||animalCare(noclick):on Dragon petted||`` event runs after the ranger completes **A … B … A … B** beside Dragon.

### What to do

**Make a ``||variables(noclick):variable||`` to remember how much love your Dragon has.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):dragonLove||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, add an ``||animalCare(noclick):on Dragon petted||`` event.

- [ ] Inside the event, place ``||variables(noclick):change dragonLove by 1||`` from ``||variables(noclick):Variables||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, add ``||animalCare(noclick):show value on Dragon's love meter||`` under ``||variables(noclick):change dragonLove by 1||`` inside the same event.

- [ ] Replace the `0` in that show block with ``||variables(noclick):dragonLove||``.

### What you should see

- [ ] Run your game.

- [ ] Stand beside Dragon with empty hands.

- [ ] Press **A … B … A … B**, with a short pause between presses.

One heart should fill in Dragon's species plaque. Simply touching the creature should not add love.

![first love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/03-first-love.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let dragonLove = 0

animalCare.onDragonPetted(function () {
    dragonLove += 1
    animalCare.showDragonLove(dragonLove)
})
```

## 4. Start the plate

Your Dragon ordered one serving of seeds. The plate needs to keep each ingredient in the order you collect it.

In the first overlap, the ranger is a sprite of kind ``||sprites(noclick):Player||`` and the prepared food is kind ``||sprites(noclick):Seeds||``. The event header calls them ``||sprites(noclick):sprite||`` and ``||sprites(noclick):otherSprite||`` in that order.

### What to do

**Make a ``||variables(noclick):variable||`` to remember what's on the plate.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):plate||``.

- [ ] Inside ``||loops(noclick):on start||``, place ``||variables(noclick):set plate to||``.

- [ ] Put the ``||arrays(noclick):empty array||`` block from **Advanced** → ``||arrays(noclick):Arrays||`` into the ``||variables(noclick):set||`` block.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):plate||`` on the plate under the ``||variables(noclick):set||`` block.

- [ ] From ``||sprites(noclick):Sprites||``, add an ``||sprites(noclick):overlap event||``.

- [ ] Choose ``||sprites(noclick):Player||`` for the first kind.

- [ ] Choose ``||sprites(noclick):Seeds||`` for the second kind.

- [ ] From **Advanced** → ``||arrays(noclick):Arrays||``, put ``||arrays(noclick):list add value to end||`` inside the ``||sprites(noclick):overlap event||``.

- [ ] Choose ``||variables(noclick):plate||`` for its list.

- [ ] Put ``||text(noclick):"seeds"||`` in its value slot.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):plate||`` on the plate inside this event.

- [ ] From ``||sprites(noclick):Sprites||``, add a ``||sprites(noclick):destroy||`` block at the end of this event.

- [ ] Drag ``||sprites(noclick):otherSprite||`` from this ``||sprites(noclick):overlap event||``'s header into the ``||sprites(noclick):destroy||`` block.

### What you should see

- [ ] Run your game.

- [ ] Press **A** once at the seed bin.

- [ ] Collect the serving that appears.

Seeds should appear in the 1st spot on the plate.

![plate: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/04-plate.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let plate: string[] = []

sprites.onOverlap(SpriteKind.Player, SpriteKind.Seeds, function (sprite, otherSprite) {
    plate.push("seeds")
    animalCare.showPlate(plate)
    otherSprite.destroy()
})

plate = []

animalCare.showPlate(plate)
```

## 5. Serve the meal

The seeds are on your plate. Now Dragon needs to eat them, and you need a fresh plate for the next order.

### What to do

**Offer the plate.**

### Add this code

- [ ] From ``||controller(noclick):Controller||``, add an ``||controller(noclick):on B button pressed||`` event.

- [ ] Inside it, use ``||animalCare(noclick):Care Displays||`` to offer ``||variables(noclick):plate||`` to the creature here.

- [ ] Under that, ``||variables(noclick):set||`` ``||variables(noclick):plate||`` to an ``||arrays(noclick):empty array||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):plate||`` on the plate.

### What you should see

- [ ] Collect seeds.

- [ ] Walk into Dragon's enclosure.

- [ ] Press **B**.

A brief **YUM!** message should appear, your plate should empty, and then, after a short rest, a new order should appear in the creature's order display. A repeated ingredient picture means another trip for another portion.

Wrong order? **B** also empties that plate so you can try again. The creature's order display will keep showing the same order.

![serve: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/05-serve.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let plate: string[] = []

controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    animalCare.servePlate(plate)
    plate = []
    animalCare.showPlate(plate)
})
```

## 6. Fill the bucket

The pump can make a full bucket, but the game needs to remember how much water you collect.

### What to do

**Make a ``||variables(noclick):variable||`` to remember how much water is in the bucket.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):bucketWater||``.

- [ ] Inside ``||loops(noclick):on start||``, ``||variables(noclick):set||`` ``||variables(noclick):bucketWater||`` to `0`.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):bucketWater||`` in the bucket under the ``||variables(noclick):set||`` block.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):FullBucket||``.

- [ ] Inside the event, ``||variables(noclick):change||`` ``||variables(noclick):bucketWater||`` by `10`.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):bucketWater||`` in the bucket inside this event.

- [ ] From ``||sprites(noclick):Sprites||``, add a ``||sprites(noclick):destroy||`` block at the end of this event.

- [ ] Put ``||sprites(noclick):otherSprite||`` from this event's header into the ``||sprites(noclick):destroy||`` block.

### What you should see

- [ ] Run your game.

- [ ] At the pump, press **A** three times with a short pause between presses: **A … A … A**.

- [ ] Walk up to collect the full bucket.

The small light beside the pump turns blue when the next beat is ready. The carried-water meter should change from `0` to `10`.

![bucket: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/06-bucket.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let bucketWater = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.FullBucket, function (sprite, otherSprite) {
    bucketWater += 10
    animalCare.showBucket(bucketWater)
    otherSprite.destroy()
})

bucketWater = 0

animalCare.showBucket(bucketWater)
```

## 7. Water Dragon

Your Dragon has its own trough. Its water must stay separate from every other creature's water.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Dragon's water.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):dragonWater||``.

- [ ] Inside ``||loops(noclick):on start||``, ``||variables(noclick):set||`` ``||variables(noclick):dragonWater||`` to `0`.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):dragonWater||`` on Dragon's water meter under the ``||variables(noclick):set||`` block.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):DragonTrough||``.

- [ ] Inside that event, ``||variables(noclick):change||`` ``||variables(noclick):dragonWater||`` by ``||variables(noclick):bucketWater||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):dragonWater||`` on Dragon's water meter.

- [ ] Then ``||variables(noclick):set||`` ``||variables(noclick):bucketWater||`` to `0`.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):bucketWater||`` in the bucket.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Dragon||`` and ``||sprites(noclick):DragonTrough||``.

- [ ] Inside that event, ``||variables(noclick):change||`` ``||variables(noclick):dragonWater||`` by `-7`.

- [ ] From ``||animalCare(noclick):Care Displays||``, show ``||variables(noclick):dragonWater||`` on Dragon's water meter.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Dragon's trough.

The bucket should empty, the trough should fill, and one drink should lower only this water meter.

![first water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/07-first-water.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let dragonWater = 0
let bucketWater = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.DragonTrough, function (sprite, otherSprite) {
    dragonWater += bucketWater
    animalCare.showDragonWater(dragonWater)
    bucketWater = 0
    animalCare.showBucket(bucketWater)
})

sprites.onOverlap(SpriteKind.Dragon, SpriteKind.DragonTrough, function (sprite, otherSprite) {
    dragonWater += -7
    animalCare.showDragonWater(dragonWater)
})

dragonWater = 0

animalCare.showDragonWater(dragonWater)
```

## 8. Give the ranger energy

Taking care of creatures is hard work. The ranger keeps its usual pace while energy is above `0`; at `0`, the exhausted ranger moves slowly. The meter has a maximum of `100`.

An ``||logic(noclick):if||`` block performs a test. If the test is true, the code inside runs. Here, the test keeps a snack from raising ``||variables(noclick):playerEnergy||`` above `100`.

### What to do

**Make a ``||variables(noclick):variable||`` to remember the ranger's energy.**

### Add this code

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):playerEnergy||``.

- [ ] Inside ``||loops(noclick):on start||``, ``||variables(noclick):set||`` ``||variables(noclick):playerEnergy||`` to `75`.

- [ ] Under it, add ``||animalCare(noclick):use value for the ranger's energy meter and speed||`` from ``||animalCare(noclick):Care Displays||``.

- [ ] Replace the `0` in that block with ``||variables(noclick):playerEnergy||``.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):Apple||``.

- [ ] Inside the event, ``||variables(noclick):change||`` ``||variables(noclick):playerEnergy||`` by `10`.

- [ ] From ``||logic(noclick):Logic||``, place an ``||logic(noclick):if true then||`` block under that change.

- [ ] In the ``||logic(noclick):if||`` block, replace `true` with the ``||logic(noclick):0 = 0||`` comparison from ``||logic(noclick):Logic||``.

- [ ] Replace the left `0` in that comparison with ``||variables(noclick):playerEnergy||``.

- [ ] Change the comparison sign from `=` to `>`.

- [ ] Change the number on the right to `100`.

- [ ] Inside the ``||logic(noclick):if||`` block, ``||variables(noclick):set||`` ``||variables(noclick):playerEnergy||`` to `100`.

- [ ] Under the ``||logic(noclick):if||`` block, add another ``||animalCare(noclick):use value for the ranger's energy meter and speed||`` block from ``||animalCare(noclick):Care Displays||``.

- [ ] Replace the `0` in that block with ``||variables(noclick):playerEnergy||``.

- [ ] ``||sprites(noclick):Destroy||`` the apple that touched the player using this event's ``||sprites(noclick):otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect an apple.

The energy meter should rise from `75` to `85`. After the apple is eaten and you step away, another can appear after about 12 seconds. Later, when energy is nearly full, an apple can restore up to `10` without taking it past `100`.

![energy: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/08-energy.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Apple, function (sprite, otherSprite) {
    playerEnergy += 10
    if (playerEnergy > 100) {
        playerEnergy = 100
    }
    animalCare.useEnergy(playerEnergy)
    otherSprite.destroy()
})

playerEnergy = 75

animalCare.useEnergy(playerEnergy)
```

## 9. Use energy while walking

The ranger should use energy when you travel, not while you stand still. A second ``||logic(noclick):if||`` test keeps the amount from dropping below `0`.

### What to do

**Change the energy after the ranger walks far enough.**

### Add this code

- [ ] From ``||animalCare(noclick):Care Displays||``, add an ``||animalCare(noclick):on ranger walking||`` event.

- [ ] Put an ``||logic(noclick):if true then||`` block inside the event.

- [ ] Make its test ask whether ``||variables(noclick):playerEnergy||`` is greater than `0`.

- [ ] Inside the ``||logic(noclick):if||`` block, ``||variables(noclick):change||`` ``||variables(noclick):playerEnergy||`` by `-1`.

- [ ] Under that change, add another ``||animalCare(noclick):use value for the ranger's energy meter and speed||`` block from ``||animalCare(noclick):Care Displays||``.

- [ ] Replace the `0` in that block with ``||variables(noclick):playerEnergy||``.

### What you should see

- [ ] Run your game.

- [ ] Walk around.

- [ ] Stand still.

- [ ] Collect an apple to restore up to `10` energy.

Walking about 45 pixels should use `1` energy. Standing still or pushing against an edge should use none. At `0`, the meter should stop decreasing, flash while you move, and the ranger should walk more slowly.

![energy timer: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/09-energy-timer.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let playerEnergy = 0

animalCare.onRangerWalk(function () {
    if (playerEnergy > 0) {
        playerEnergy += -1
        animalCare.useEnergy(playerEnergy)
    }
})
```

## 10. Bring in Unicorn

Your 2nd enclosure is ready for Unicorn.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your 2nd creature.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):animal2||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):animal2||`` to ``||text(noclick):"Unicorn"||`` in ``||loops(noclick):on start||``.

- [ ] Show ``||variables(noclick):animal2||`` in the 2nd enclosure with ``||animalCare(noclick):Care Displays||``.

### What you should see

- [ ] Run your game.

Unicorn should enter the 2nd enclosure without replacing Dragon.

![second arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/10-second-arrival.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let animal2 = ""

animal2 = "Unicorn"

animalCare.showAnimal2(animal2)
```

## 11. Name and love Unicorn

Your new arrival needs its own name and its own hearts.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Unicorn's name.**

**Make a ``||variables(noclick):variable||`` to remember how much love your Unicorn has.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):unicornName||``.

- [ ] In ``||loops(noclick):on start||``, under the block that shows ``||variables(noclick):animal2||`` in the 2nd enclosure, ``||variables(noclick):set||`` ``||variables(noclick):unicornName||`` to `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] Show ``||variables(noclick):unicornName||`` beside Unicorn with ``||animalCare(noclick):Care Displays||``.

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):unicornLove||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, add an ``||animalCare(noclick):on Unicorn petted||`` event.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):unicornLove||`` by `1`.

- [ ] With ``||animalCare(noclick):Care Displays||``, add ``||animalCare(noclick):show value on Unicorn's love meter||`` under that change.

- [ ] Replace the `0` in that show block with ``||variables(noclick):unicornLove||``.

### What you should see

- [ ] Run your game.

- [ ] Empty your plate.

- [ ] Stand beside Unicorn.

- [ ] Press **A … B … A … B** with short pauses.

The new name should stay with Unicorn, and one completed pet should fill only its heart meter.

![second name love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/11-second-name-love.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let unicornName = ""
let unicornLove = 0

animalCare.onUnicornPetted(function () {
    unicornLove += 1
    animalCare.showUnicornLove(unicornLove)
})

unicornName = "Nova"

animalCare.showUnicornName(unicornName)
```

## 12. Add berries to the plate

Unicorn ordered berries, then seeds.

### What to do

**Keep the new ingredient on the same plate.**

### Make this happen

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):Berries||``.

- [ ] Inside it, add ``||text(noclick):"berries"||`` to the end of ``||variables(noclick):plate||`` with ``||arrays(noclick):Arrays||``.

- [ ] Show ``||variables(noclick):plate||`` on the plate with ``||animalCare(noclick):Care Displays||``.

- [ ] ``||sprites(noclick):Destroy||`` the berries that were collected using this event's ``||sprites(noclick):otherSprite||``.

### What you should see

- [ ] Hold **A** at the berry station until the serving appears.

- [ ] Collect berries.

- [ ] Collect seeds next.

- [ ] Carry the plate into Unicorn's enclosure.

- [ ] Press **B**.

The plate should show berries, then seeds. A brief **YUM!** message should appear. After a short rest, another order should appear in the creature's order display.

![berries: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/12-berries.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let plate: string[] = []

sprites.onOverlap(SpriteKind.Player, SpriteKind.Berries, function (sprite, otherSprite) {
    plate.push("berries")
    animalCare.showPlate(plate)
    otherSprite.destroy()
})
```

## 13. Water Unicorn

Two creatures, two troughs. This pour belongs to Unicorn.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Unicorn's water.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):unicornWater||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):unicornWater||`` to `0` in ``||loops(noclick):on start||``.

- [ ] Show ``||variables(noclick):unicornWater||`` on Unicorn's water meter with ``||animalCare(noclick):Care Displays||``.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):UnicornTrough||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):unicornWater||`` by ``||variables(noclick):bucketWater||``.

- [ ] Show ``||variables(noclick):unicornWater||`` on Unicorn's water meter with ``||animalCare(noclick):Care Displays||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):bucketWater||`` to `0`.

- [ ] Show ``||variables(noclick):bucketWater||`` in the bucket with ``||animalCare(noclick):Care Displays||``.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Unicorn||`` and ``||sprites(noclick):UnicornTrough||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):unicornWater||`` by `-4`.

- [ ] Show ``||variables(noclick):unicornWater||`` on Unicorn's water meter with ``||animalCare(noclick):Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Unicorn's trough.

Only Unicorn's water meter should move.

![second water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/13-second-water.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let unicornWater = 0
let bucketWater = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.UnicornTrough, function (sprite, otherSprite) {
    unicornWater += bucketWater
    animalCare.showUnicornWater(unicornWater)
    bucketWater = 0
    animalCare.showBucket(bucketWater)
})

sprites.onOverlap(SpriteKind.Unicorn, SpriteKind.UnicornTrough, function (sprite, otherSprite) {
    unicornWater += -4
    animalCare.showUnicornWater(unicornWater)
})

unicornWater = 0

animalCare.showUnicornWater(unicornWater)
```

## 14. Add a stronger energy food

A sandwich can restore more energy than an apple, but energy still stops at `100`.

### What to do

**Make the sandwich add more energy.**

### Make this happen

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):Sandwich||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):playerEnergy||`` by `25`.

- [ ] Under that change, add the same ``||logic(noclick):if||`` test that checks whether ``||variables(noclick):playerEnergy||`` is greater than `100`.

- [ ] Inside the ``||logic(noclick):if||`` block, ``||variables(noclick):set||`` ``||variables(noclick):playerEnergy||`` to `100`.

- [ ] Under the ``||logic(noclick):if||`` block, add another ``||animalCare(noclick):use value for the ranger's energy meter and speed||`` block from ``||animalCare(noclick):Care Displays||``.

- [ ] Replace the `0` in that block with ``||variables(noclick):playerEnergy||``.

- [ ] ``||sprites(noclick):Destroy||`` the sandwich using this event's ``||sprites(noclick):otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect a sandwich.

- [ ] Compare the meter change with the apple's smaller boost.

With enough room in the meter, the sandwich should add `25` energy. Near full, it should stop at `100`. After it is eaten and you step away, another can appear after about 30 seconds.

![sandwich energy: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/14-second-creature.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Sandwich, function (sprite, otherSprite) {
    playerEnergy += 25
    if (playerEnergy > 100) {
        playerEnergy = 100
    }
    animalCare.useEnergy(playerEnergy)
    otherSprite.destroy()
})
```

## 15. Bring in Phoenix

The last roster card shows Phoenix.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your 3rd creature.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):animal3||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):animal3||`` to ``||text(noclick):"Phoenix"||`` in ``||loops(noclick):on start||``.

- [ ] Show ``||variables(noclick):animal3||`` in the 3rd enclosure with ``||animalCare(noclick):Care Displays||``.

### What you should see

- [ ] Run your game.

All three creatures should now have their own enclosure.

![third arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/15-third-arrival.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let animal3 = ""

animal3 = "Phoenix"

animalCare.showAnimal3(animal3)
```

## 16. Name and love Phoenix

Phoenix still needs a name and love of its own.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Phoenix's name.**

**Make a ``||variables(noclick):variable||`` to remember how much love your Phoenix has.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):phoenixName||``.

- [ ] In ``||loops(noclick):on start||``, under the block that shows ``||variables(noclick):animal3||`` in the 3rd enclosure, ``||variables(noclick):set||`` ``||variables(noclick):phoenixName||`` to `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] Show ``||variables(noclick):phoenixName||`` beside Phoenix with ``||animalCare(noclick):Care Displays||``.

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):phoenixLove||``.

- [ ] From ``||animalCare(noclick):Care Displays||``, add an ``||animalCare(noclick):on Phoenix petted||`` event.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):phoenixLove||`` by `1`.

- [ ] Add ``||animalCare(noclick):show value on Phoenix's love meter||`` under that change.

- [ ] Replace the `0` in that show block with ``||variables(noclick):phoenixLove||``.

### What you should see

- [ ] Run your game.

- [ ] Empty your plate.

- [ ] Stand beside Phoenix.

- [ ] Press **A … B … A … B** with short pauses.

The name and heart meter should belong to Phoenix. Touching it without the petting pattern should not add a heart.

![third name love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/16-third-name-love.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let phoenixName = ""
let phoenixLove = 0

animalCare.onPhoenixPetted(function () {
    phoenixLove += 1
    animalCare.showPhoenixLove(phoenixLove)
})

phoenixName = "Clover"

animalCare.showPhoenixName(phoenixName)
```

## 17. Add greens to the plate

Phoenix ordered greens, berries, then seeds.

### What to do

**Keep all three ingredients in their collected order.**

### Make this happen

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):Greens||``.

- [ ] Inside it, add ``||text(noclick):"greens"||`` to the end of ``||variables(noclick):plate||`` with ``||arrays(noclick):Arrays||``.

- [ ] Show ``||variables(noclick):plate||`` on the plate with ``||animalCare(noclick):Care Displays||``.

- [ ] ``||sprites(noclick):Destroy||`` the collected serving using this event's ``||sprites(noclick):otherSprite||``.

### What you should see

- [ ] Tap **A** three times at the greens station.

- [ ] Collect greens.

- [ ] Collect berries next.

- [ ] Collect seeds last.

- [ ] Check all three plate spots.

- [ ] Offer the finished plate to Phoenix with **B**.

The plate should keep greens, berries, then seeds in that order.

![greens: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/17-greens.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let plate: string[] = []

sprites.onOverlap(SpriteKind.Player, SpriteKind.Greens, function (sprite, otherSprite) {
    plate.push("greens")
    animalCare.showPlate(plate)
    otherSprite.destroy()
})
```

## 18. Water Phoenix

One last trough. Phoenix takes a different-sized drink.

### What to do

**Make a ``||variables(noclick):variable||`` to remember your Phoenix's water.**

### Make this happen

- [ ] Make a new ``||variables(noclick):variable||`` named ``||variables(noclick):phoenixWater||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):phoenixWater||`` to `0` in ``||loops(noclick):on start||``.

- [ ] Show ``||variables(noclick):phoenixWater||`` on Phoenix's water meter with ``||animalCare(noclick):Care Displays||``.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):PhoenixTrough||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):phoenixWater||`` by ``||variables(noclick):bucketWater||``.

- [ ] Show ``||variables(noclick):phoenixWater||`` on Phoenix's water meter with ``||animalCare(noclick):Care Displays||``.

- [ ] ``||variables(noclick):Set||`` ``||variables(noclick):bucketWater||`` to `0`.

- [ ] Show ``||variables(noclick):bucketWater||`` in the bucket with ``||animalCare(noclick):Care Displays||``.

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Phoenix||`` and ``||sprites(noclick):PhoenixTrough||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):phoenixWater||`` by `-3`.

- [ ] Show ``||variables(noclick):phoenixWater||`` on Phoenix's water meter with ``||animalCare(noclick):Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Phoenix's trough.

The Phoenix meter should change; the other two water meters should not.

![third water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/18-third-water.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let phoenixWater = 0
let bucketWater = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.PhoenixTrough, function (sprite, otherSprite) {
    phoenixWater += bucketWater
    animalCare.showPhoenixWater(phoenixWater)
    bucketWater = 0
    animalCare.showBucket(bucketWater)
})

sprites.onOverlap(SpriteKind.Phoenix, SpriteKind.PhoenixTrough, function (sprite, otherSprite) {
    phoenixWater += -3
    animalCare.showPhoenixWater(phoenixWater)
})

phoenixWater = 0

animalCare.showPhoenixWater(phoenixWater)
```

## 19. Add the strongest energy food

Cake can restore up to `50` energy, the largest snack boost.

### What to do

**Make cake give the biggest energy boost.**

### Make this happen

- [ ] Add an ``||sprites(noclick):overlap event||`` for ``||sprites(noclick):Player||`` and ``||sprites(noclick):Cake||``.

- [ ] Inside it, ``||variables(noclick):change||`` ``||variables(noclick):playerEnergy||`` by `50`.

- [ ] Under that change, add the same ``||logic(noclick):if||`` test that checks whether ``||variables(noclick):playerEnergy||`` is greater than `100`.

- [ ] Inside the ``||logic(noclick):if||`` block, ``||variables(noclick):set||`` ``||variables(noclick):playerEnergy||`` to `100`.

- [ ] Under the ``||logic(noclick):if||`` block, add another ``||animalCare(noclick):use value for the ranger's energy meter and speed||`` block from ``||animalCare(noclick):Care Displays||``.

- [ ] Replace the `0` in that block with ``||variables(noclick):playerEnergy||``.

- [ ] ``||sprites(noclick):Destroy||`` the cake using this event's ``||sprites(noclick):otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect cake.

- [ ] Compare the three possible boosts: apple `10`, sandwich `25`, and cake `50`.

With at least `50` empty points, cake should add `50`. Near full, it should stop at `100`. After it is eaten and you step away, another can appear after about 60 seconds.

![cake energy: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/19-complete.gif)

#### ~ tutorialhint

```blocks
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Cake, function (sprite, otherSprite) {
    playerEnergy += 50
    if (playerEnergy > 100) {
        playerEnergy = 100
    }
    animalCare.useEnergy(playerEnergy)
    otherSprite.destroy()
})
```

## Final shift

All three enclosures are open.

### What to do

**Complete your first shift.**

- [ ] Serve each creature's ordered plate with **B**.

- [ ] Fill each trough.

- [ ] Watch each creature take a drink.

- [ ] Pet every creature with **A … B … A … B** while your plate is empty.

- [ ] Eat a snack after walking uses some energy.

### What you should see

Each creature's order display shows its recipe from left to right. One ingredient picture means one portion and one collection trip, so repeated pictures mean repeated trips. When your plate exactly matches a ready order, that creature's feeding plate should flash. **A** prepares at a station. In an enclosure, **B** offers a nonempty plate; with empty hands, **A … B … A … B** pets the nearby creature.

- [ ] Walk up from a station to collect the food or water it prepares.

- [ ] Watch the creature names, plate spots, water meters, heart meters, and energy meter while you play.

Taking care of one creature should not quietly change another creature's values. Hearts should appear beside each species name without a separate love number. When all three creatures have eaten, had a drink, and received love, and you have used and restored some energy, **FIRST SHIFT COMPLETE!** should appear.


![The completed first shift](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/28872848a75c/20-final-shift.gif)

## What did we learn?

Every time the game needed to remember something new, you made a ``||variables(noclick):variable||`` for it.

You ``||variables(noclick):set||`` creature choices and names by replacing what the ``||variables(noclick):variable||`` held. You ``||variables(noclick):changed||`` water, love, and energy by adding or removing an amount. You added each ingredient to ``||variables(noclick):plate||`` without removing the ingredients already there.

You also used ``||logic(noclick):if||`` tests to keep ``||variables(noclick):playerEnergy||`` between `0` and `100` while the learner-owned value still caused every visible energy change.

Look at your ``||variables(noclick):Variables||`` toolbox. How many of those ``||variables(noclick):variables||`` did not exist before the game needed them?

```template
namespace SpriteKind {
    export const Dragon = SpriteKind.create()
    export const Unicorn = SpriteKind.create()
    export const Phoenix = SpriteKind.create()
    export const DragonTrough = SpriteKind.create()
    export const UnicornTrough = SpriteKind.create()
    export const PhoenixTrough = SpriteKind.create()
    export const Seeds = SpriteKind.create()
    export const Berries = SpriteKind.create()
    export const Greens = SpriteKind.create()
    export const FullBucket = SpriteKind.create()
    export const Apple = SpriteKind.create()
    export const Sandwich = SpriteKind.create()
    export const Cake = SpriteKind.create()
}
```

```customts
namespace userconfig {
    export const ARCADE_SCREEN_WIDTH = 320
    export const ARCADE_SCREEN_HEIGHT = 240
}

//% color=#6d4fc2 icon="\uf06e" block="Care Displays"
namespace animalCare {
    const chosen = ["Dragon", "Unicorn", "Phoenix"]
    const homeX = [31, 137, 243]
    const troughX = [88, 194, 300]
    const stationX = [30, 77, 124, 174]
    const snackX = [256, 278, 300]
    const snackY = 195
    const costs = [Math.abs(-7), Math.abs(-4), Math.abs(-3)]
    let ingredientKinds: number[] = []
    let snackKinds: number[] = []
    const words = ["seeds", "berries", "greens", "water", "apple", "sandwich", "cake"]
    const snackCooldownMs = [12000, 30000, 60000]
    let snackReadyAt = [0, 0, 0]
    let ranger: Sprite = null
    let creatures: Sprite[] = [null, null, null]
    let creatureKinds = [0, 0, 0]
    let admitted = [false, false, false]
    let reportedNames = ["", "", ""]
    let reportedLove = [0, 0, 0]
    let reportedWater = [0, 0, 0]
    let reportedPlate: string[] = []
    let reportedBucket = 0
    let reportedEnergy = 0
    let energyShown = false
    let ateEnergyFood = false
    let energyDecayed = false
    let petHandlers: (() => void)[] = [null, null, null]
    let walkingHandler: () => void = null
    let petSlot = -1
    let petStrokes = 0
    let lastPetAt = -5000
    let petReadyAt = 0
    let lastRangerX = 160
    let lastRangerY = 155
    let walkingDistance = 0
    let movingUntil = 0
    let drinking = [false, false, false]
    let returning = [false, false, false]
    let drank = [false, false, false]
    let meals = [0, 0, 0]
    let orders: string[][] = [["seeds"], ["berries", "seeds"], ["greens", "berries", "seeds"]]
    let servedUntil = [0, 0, 0]
    let nextMealAt = [0, 0, 0]
    let orderReady = [false, false, false]
    let orderVisible = [false, false, false]
    let plateMatchShown = [false, false, false]
    const mealRestMs = 12000
    let knownIngredients = 0
    let nextDrink = [0, 0, 0]
    let unlocked = 0
    let berryHoldAt = 0
    let berryPrepared = false
    let greensTaps = 0
    let lastGreenTapAt = 0
    let pumpBeats = 0
    let lastPumpBeatAt = 0
    let pumpStrokeAt = -5000
    let pumpStrokeValid = false
    let energyGainImages: Image[] = []
    let energyGainX: number[] = []
    let energyGainY: number[] = []
    let energyGainAt: number[] = []
    let statusText = "Welcome, ranger!"
    let statusUntil = 2500
    let worldStarted = false
    let shiftWon = false
    let creatureFrames: Image[][] = [[], [], []]
    let rangerFrames: Image[] = []
    let rangerFacing = 0
    let affectionAt = [-5000, -5000, -5000]
    let waterAt = [-5000, -5000, -5000]

    // All frames are supplied art. They never set or change learner values.
    function creatureFrame(base: Image, mark: string, phase: number, blink: boolean): Image {
        let p = image.create(base.width, base.height)
        let sway = phase == 1 ? -1 : phase == 3 ? 1 : 0
        for (let y = 0; y < base.height; y++) {
            for (let x = 0; x < base.width; x++) {
                let color = base.getPixel(x, y)
                if (color == 0) continue
                let dx = 0
                let dy = 0
                if (mark == "wings" && x > 2 && x < 12 && y > 4 && y < 13) dy = sway
                if (mark == "wings" && x < 7 && y > 14 && y < 18) dy = -sway
                if (mark == "horn" && color == 10 && y > 6 && y < 16) dx = sway
                if (mark == "flame" && (x < 8 || x > 16) && y > 6 && y < 14) dy = sway
                if (mark == "flame" && y > 16 && y < base.height - 1) dx = sway
                // Blink closes an existing eye, without adding a collision pixel.
                if (blink && color == 15) color = mark == "horn" ? 14 : mark == "flame" ? 4 : mark == "wings" ? 2 : 14
                p.setPixel(Math.max(0, Math.min(base.width - 1, x + dx)), Math.max(0, Math.min(base.height - 1, y + dy)), color)
            }
        }
        // Preserve all outermost nontransparent pixels across frames so the
        // animation cannot enlarge or shrink the actor's collision bounds.
        let left = base.width, right = 0, top = base.height, bottom = 0
        for (let y = 0; y < base.height; y++) for (let x = 0; x < base.width; x++) {
            if (base.getPixel(x, y) != 0) { left = Math.min(left, x); right = Math.max(right, x); top = Math.min(top, y); bottom = Math.max(bottom, y) }
        }
        for (let y = 0; y < base.height; y++) for (let x = 0; x < base.width; x++) {
            if (x < left || x > right || y < top || y > bottom) p.setPixel(x, y, 0)
            else if ((x == left || x == right || y == top || y == bottom) && base.getPixel(x, y) != 0) p.setPixel(x, y, base.getPixel(x, y))
        }
        return p
    }

    function walkingFrame(direction: number, phase: number): Image {
        let p = rangerImage()
        // Face, hat band and backpack distinguish all four directions.
        if (direction == 1) {
            p.fillRect(5, 6, 7, 4, 14)
            p.fillRect(5, 11, 7, 5, 4); p.drawRect(5, 11, 7, 5, 14)
            p.fillRect(7, 12, 3, 2, 5)
        } else if (direction > 1) {
            p.fillRect(5, 6, 7, 4, 13)
            p.fillRect(direction == 2 ? 10 : 5, 6, 2, 4, 14)
            p.setPixel(direction == 2 ? 6 : 10, 7, 15)
            p.fillRect(direction == 2 ? 3 : 11, 11, 3, 5, 4)
        }
        if (phase == 1 || phase == 3) {
            p.fillRect(4, 16, 9, 4, 0)
            let shortLeg = phase == 1 ? 5 : 9
            let longLeg = phase == 1 ? 9 : 5
            p.fillRect(shortLeg, 16, 3, 1, 8)
            p.fillRect(shortLeg == 5 ? 4 : 9, 17, 4, 2, 14)
            p.fillRect(longLeg, 16, 3, 3, 8)
            p.fillRect(longLeg == 5 ? 4 : 9, 19, 4, 1, 14)
            p.fillRect(phase == 1 ? 3 : 13, 12, 1, 2, 6)
        }
        return p
    }

    function art(rows: string[]): Image {
        let width = 0
        for (let row of rows) width = Math.max(width, row.length)
        let result = image.create(width, rows.length)
        for (let y = 0; y < rows.length; y++) {
            for (let x = 0; x < rows[y].length; x++) {
                if (rows[y].charAt(x) != ".") result.setPixel(x, y, parseInt(rows[y].charAt(x), 16))
            }
        }
        return result
    }

    function creatureImage(body: number, accent: number, mark: string): Image {
        if (mark == "horn") return art([
            "....................5...", "...................55...", "..................d5....",
            "...............a.dddd...", "..............aaadddddd.", "..............aaddfdddd.",
            ".............aadddddddd.", "............aaadddddd...", "...aa......aaaddddd.....",
            "..aaa....dddddddddd.....", ".aaaa..ddddddddddddd....", ".aaa..dddddddddddddd....",
            "..aa.ddddddddddddddd....", "...a.dddd1dddddddddd....", ".....dddd11dddddddd.....",
            ".....dddddddddddddd.....", "......ddd.....dddd......", "......ddd......ddd......",
            "......ddd......ddd......", "......aaa......aaa......", "......aaa......aaa......"
        ])
        if (mark == "flame") return art([
            "............4...........", "...........454..........", "..........4554..........",
            "..........454...........", "...4......444......4....", "...44....44444....44....",
            "..4454...44f445..4544...", "..44554..44445..45544...", ".44455544444444555444...",
            ".24455554444445555442...", ".22445555444455554422...", "..22445554445554422....",
            "...224454444444422......", "....2244444444422.......", "......244454442.........",
            "........44544...........", ".......2445442..........", "......244454442.........",
            ".....2444.5.4442........", ".....244..5..442........", "......24..4..42.........",
            ".......2.....2.........."
        ])
        if (mark == "wings") return art([
            "................5..5....", "...2...........22522....", "...22.........2222222...",
            "...2522.......222f2222..", "...255222.....222222222.", "...2555222....224444222.",
            "...25555222...224444....", "...255555222..22224.....", "...2552552222222222.....",
            "...22522522222222222....", "....2222222222444222....", ".....222222222444422....",
            ".....222222224444422....", "..2..222222224444422....", ".22..222222224444422....",
            ".222222222222444422.....", "..2222222222224422......", "...222222222222222......",
            ".......2222...2222......", ".......2222...2222......", ".......5555...5555......"
        ])
        let picture = image.create(26, 24)
        picture.fillCircle(13, 13, 9, body)
        picture.fillCircle(14, 15, 6, accent)
        picture.fillCircle(9, 5, 4, body)
        picture.fillCircle(18, 5, 4, body)
        picture.fillRect(7, 19, 4, 4, body)
        picture.fillRect(17, 19, 4, 4, body)
        picture.fillRect(9, 9, 2, 3, 15)
        picture.fillRect(17, 9, 2, 3, 15)
        if (mark == "trunk") picture.fillRect(12, 11, 3, 12, body)
        if (mark == "spikes") {
            for (let i = 0; i < 4; i++) picture.fillRect(2 + i * 3, 2 + i, 2, 5, accent)
        }
        if (mark == "shell") picture.drawCircle(13, 14, 7, 15)
        return picture
    }

    function rangerImage(): Image {
        return art([
            "......44444......", ".....4444444.....", "....444555444....", "....444444444....",
            "..4444444444444..", "...eeeeeeeeeee...", ".....ddddddd.....", ".....dfdddfd.....",
            ".....ddddddd.....", "......deeed......", "....666666666....", "...d666666666d...",
            "...d666566666d...", "...d666666666d...", "....666666666....", ".....8888888.....",
            ".....888.888.....", ".....888.888.....", ".....eee.eee.....", "....eeee.eeee...."
        ])
    }

    function itemImage(word: string): Image {
        let p = image.create(15, 15)
        if (word == "seeds") {
            // The same bounded packet and grain strokes appear everywhere.
            p.fillRect(1, 1, 13, 13, 14); p.fillRect(2, 2, 11, 11, 13)
            p.drawLine(2, 2, 12, 2, 5); p.drawLine(2, 12, 12, 12, 4)
            for (let row = 0; row < 2; row++) for (let seed = 0; seed < 3; seed++) {
                let sx = 3 + seed * 3, sy = 4 + row * 4
                p.drawLine(sx, sy + 2, sx + 1, sy, 5); p.setPixel(sx, sy + 1, 4)
            }
        } else if (word == "berries") {
            p.fillCircle(7, 8, 6, 2); p.fillCircle(8, 9, 4, 3)
            p.drawLine(7, 4, 8, 1, 14); p.drawLine(8, 2, 11, 1, 7)
            p.fillRect(4, 5, 2, 2, 1); p.setPixel(3, 7, 3)
        } else if (word == "greens") {
            oval(p, 2, 2, 7, 10, 6); oval(p, 6, 0, 8, 12, 7)
            p.drawLine(7, 14, 10, 3, 5); p.drawLine(7, 12, 4, 4, 5)
            p.drawLine(9, 7, 12, 5, 6)
        } else if (word == "water") {
            p.drawRect(3, 1, 9, 9, 11); p.fillRect(2, 6, 11, 8, 8)
            p.fillRect(3, 7, 9, 5, 9); p.drawLine(4, 8, 9, 8, 1)
        } else if (word == "apple") {
            p.fillCircle(5, 9, 4, 2); p.fillCircle(10, 9, 4, 2)
            p.fillRect(7, 2, 2, 4, 14); p.drawLine(9, 3, 12, 1, 6); p.fillRect(4, 6, 2, 2, 1)
        } else if (word == "sandwich") {
            // Rounded bread, dark crust and separate lettuce/tomato/cheese layers.
            oval(p, 1, 2, 13, 6, 4); oval(p, 2, 2, 11, 4, 13)
            p.drawLine(3, 3, 10, 3, 1)
            p.fillRect(1, 7, 13, 2, 7); p.setPixel(3, 9, 7); p.setPixel(11, 9, 7)
            p.fillRect(2, 9, 11, 2, 2); p.fillRect(3, 10, 10, 2, 5)
            p.fillRect(1, 12, 13, 2, 4); p.drawLine(2, 12, 12, 12, 13)
        } else {
            // Frosted cake slice, sponge layers and a cherry, not a soup bowl.
            p.fillRect(2, 6, 12, 8, 4); p.fillRect(3, 7, 10, 6, 5)
            p.fillRect(2, 9, 12, 2, 3); p.fillRect(2, 5, 12, 3, 1)
            p.drawLine(3, 4, 10, 2, 1); p.drawLine(3, 5, 13, 5, 1)
            p.fillCircle(9, 3, 2, 2); p.setPixel(9, 0, 7)
            p.drawLine(1, 14, 14, 14, 11)
        }
        return p
    }

    function oval(p: Image, x: number, y: number, width: number, height: number, color: number) {
        for (let row = 0; row < height; row++) {
            let dy = (row + 0.5 - height / 2) / (height / 2)
            let half = Math.sqrt(Math.max(0, 1 - dy * dy)) * width / 2
            p.drawLine(Math.ceil(x + width / 2 - half), y + row, Math.floor(x + width / 2 + half), y + row, color)
        }
    }

    function fence(p: Image, x: number, y: number, length: number) {
        p.fillRect(x, y + 5, length, 2, 14)
        p.fillRect(x, y + 4, length, 1, 4)
        for (let post = x; post < x + length; post += 11) {
            p.fillRect(post, y + 2, 4, 12, 14)
            p.fillRect(post, y + 1, 3, 10, 4)
            p.fillRect(post + 1, y, 1, 10, 5)
        }
    }

    function flower(p: Image, x: number, y: number, color: number) {
        // A cupped tulip with a visible green stalk and leaves, not a text glyph.
        p.drawLine(x + 1, y + 2, x + 1, y + 9, 12)
        p.drawLine(x, y + 2, x, y + 9, 7)
        oval(p, x - 5, y + 4, 5, 2, 7); oval(p, x + 1, y + 6, 4, 2, 7)
        oval(p, x - 3, y - 2, 7, 6, color)
        p.drawLine(x - 3, y - 3, x - 3, y, color)
        p.drawLine(x, y - 4, x, y, color)
        p.drawLine(x + 3, y - 3, x + 3, y, color)
        p.drawLine(x - 1, y - 1, x - 1, y + 1, color == 1 ? 5 : 1)
    }

    function stone(p: Image, x: number, y: number, width: number, height: number) {
        // Small separate stones leave grass showing around and between them.
        oval(p, x, y + 2, width, height, 12)
        oval(p, x, y, width, height, 11)
        p.drawLine(x + 3, y + 2, x + Math.idiv(width, 2), y + 1, 13)
        p.drawLine(x + Math.idiv(width, 2) + 2, y + 3, x + Math.idiv(width, 2), y + 5, 12)
        p.setPixel(x + width - 5, y + height - 3, 12)
        p.setPixel(x + 5, y + height - 2, 13)
    }

    function habitat(p: Image, slot: number) {
        let x = slot * 106 + 4
        // Grass clearings and open fences: no panel background or card border.
        oval(p, x + 6, 53, 86, 62, 7)
        oval(p, x + 14, 71, 60, 28, 6)
        // The controls keep their strip; the enclosure begins immediately below.
        fence(p, x, 24, 99)
        for (let y = 37; y < 121; y += 18) {
            p.fillRect(x, y, 3, 12, 14); p.fillRect(x, y, 2, 9, 4)
        }
        fence(p, x, 120, 17); fence(p, x + 61, 122, 38)
        // A real entrance, with stepping stones leading into the habitat.
        stone(p, x + 23, 121, 17, 7); stone(p, x + 30, 132, 19, 6)
        if (slot == 0) {
            // Warm stone sleeping nook and a few little crystals.
            oval(p, x + 6, 45, 32, 25, 11)
            p.fillCircle(x + 16, 57, 11, 12); p.fillCircle(x + 25, 57, 10, 11)
            oval(p, x + 13, 53, 17, 17, 14); oval(p, x + 16, 57, 13, 12, 15)
            p.drawLine(x + 10, 50, x + 16, 47, 1)
            p.drawLine(x + 22, 49, x + 30, 51, 13)
            p.fillRect(x + 81, 53, 4, 13, 10); p.drawLine(x + 81, 53, x + 83, 49, 3)
            p.fillRect(x + 85, 59, 4, 8, 3); p.setPixel(x + 82, 53, 1)
        } else if (slot == 1) {
            // Flowering resting grove shares the Dragon den's top-left footprint.
            oval(p, x + 6, 45, 32, 25, 6)
            p.fillRect(x + 18, 53, 4, 15, 14); p.drawLine(x + 20, 57, x + 12, 50, 14)
            p.fillCircle(x + 16, 47, 9, 7); p.fillCircle(x + 28, 49, 9, 7)
            p.fillCircle(x + 23, 44, 8, 6)
            flower(p, x + 11, 58, 3); flower(p, x + 31, 59, 1)
        } else {
            // Woven resting nest in the same top-left den area.
            oval(p, x + 6, 49, 34, 20, 14); oval(p, x + 8, 47, 30, 18, 4)
            oval(p, x + 12, 49, 22, 11, 5); oval(p, x + 15, 50, 16, 7, 14)
            for (let i = 0; i < 4; i++) p.drawLine(x + 9 + i * 7, 58, x + 13 + i * 7, 66, 5)
            p.fillRect(x + 79, 55, 3, 14, 14); p.fillRect(x + 72, 53, 20, 3, 4)
            flower(p, x + 10, 57, 4); flower(p, x + 88, 67, 5)
        }
        flower(p, x + 9, 115, slot == 1 ? 3 : 5)
        flower(p, x + 91, 114, 1)
        // Trough feet and cast shadow belong to the landscape; the existing
        // overlap sprite stays centered on the actual water bowl.
        oval(p, troughX[slot] - 11, 75, 23, 37, 6)
        p.fillRect(troughX[slot] - 7, 104, 3, 6, 14)
        p.fillRect(troughX[slot] + 4, 104, 3, 6, 14)
        // A separate feeding plate on a woven mat, left of the water station.
        p.fillRect(x + 15, 112, 48, 13, 14)
        p.fillRect(x + 16, 112, 46, 11, 4)
        for (let stitch = 0; stitch < 7; stitch++) p.drawLine(x + 18 + stitch * 6, 113, x + 20 + stitch * 6, 122, 5)
        oval(p, x + 18, 114, 42, 10, 11)
        oval(p, x + 18, 112, 42, 10, 1)
        oval(p, x + 22, 114, 34, 6, 13)
    }

    function makeBackground(): Image {
        let p = image.create(320, 240)
        p.fill(6)
        for (let y = 26; y < 219; y += 19) {
            for (let x = 7 + y % 11; x < 320; x += 31) {
                p.drawLine(x, y, x + 2, y - 2, 7)
            }
        }
        p.fillRect(0, 0, 320, 22, 15); p.fillRect(0, 22, 320, 2, 5)
        for (let i = 0; i < 9; i++) {
            let x = 8 + i * 35
            stone(p, x, 146 + i % 3 * 5, 19 + i % 2 * 3, 8)
            if (i % 2 == 0) stone(p, x + 13, 166, 14, 6)
            flower(p, x + 10, 177, i % 3 == 0 ? 3 : 1)
        }
        for (let slot = 0; slot < 3; slot++) habitat(p, slot)
        fence(p, 316, 24, 4)
        for (let i = 0; i < 3; i++) drawIngredientBin(p, i)
        // A small wooden table, with actual collectible food on its surface.
        oval(p, 239, 212, 78, 6, 6)
        p.fillRect(245, 207, 4, 11, 14); p.fillRect(307, 207, 4, 11, 14)
        p.fillRect(246, 210, 2, 6, 4); p.fillRect(307, 210, 2, 6, 4)
        p.fillRect(250, 200, 4, 13, 14); p.fillRect(301, 200, 4, 13, 14)
        p.fillRect(240, 198, 76, 15, 14)
        p.fillRect(241, 197, 74, 12, 4); p.drawLine(242, 197, 313, 197, 5)
        p.drawLine(242, 203, 313, 203, 14); p.drawLine(242, 208, 313, 208, 5)
        p.drawLine(267, 198, 266, 201, 14); p.drawLine(293, 204, 293, 207, 14)
        for (let i = 0; i < 3; i++) oval(p, snackX[i] - 9, 200, 18, 4, 13)
        p.fillRect(0, 219, 320, 21, 15)
        return p
    }

    function drawIngredientBin(p: Image, index: number) {
        let x = stationX[index] - 19
        oval(p, x - 2, 202, 43, 8, 6)
        // Open dark interior, raised rim, front slats and two visible feet.
        p.fillRect(x + 3, 204, 4, 5, 14); p.fillRect(x + 31, 204, 4, 5, 14)
        p.fillRect(x, 184, 39, 21, 14); p.fillRect(x + 2, 186, 35, 11, 15)
        let ingredient = itemImage(words[index])
        p.drawTransparentImage(ingredient, x + 2, 179)
        p.drawTransparentImage(ingredient, x + 21, 180)
        p.drawTransparentImage(ingredient, x + 12, 183)
        p.drawLine(x, 196, x + 38, 196, 5)
        p.fillRect(x + 1, 197, 37, 9, 4)
        p.drawLine(x + 2, 201, x + 36, 201, 14)
        p.drawLine(x + 2, 205, x + 36, 205, 5)
        p.fillRect(x + 3, 196, 3, 10, 14); p.fillRect(x + 32, 196, 3, 10, 14)
        p.setPixel(x + 4, 198, 11); p.setPixel(x + 33, 198, 11)
    }

    function drawPump() {
        let x = stationX[3]
        oval(screen, x - 24, 203, 48, 7, 6)
        screen.fillRect(x - 8, 202, 20, 5, 14)
        screen.fillRect(x - 6, 200, 16, 4, 11)
        screen.fillRect(x - 3, 181, 9, 21, 8)
        screen.fillRect(x - 1, 182, 3, 18, 9)
        screen.fillCircle(x + 1, 180, 6, 8)
        screen.drawLine(x - 3, 177, x + 3, 177, 11)
        screen.fillRect(x - 13, 182, 13, 4, 8)
        screen.fillRect(x - 15, 183, 4, 6, 8)
        screen.drawLine(x - 12, 183, x - 5, 183, 9)
        // Accepted strokes keep their animation even when the third beat resets
        // preparation. Neither animation nor water flow collects the bucket.
        let age = control.millis() - pumpStrokeAt
        let dip = age < 160 ? Math.idiv(age * 18, 160) : age < 400 ? Math.idiv((400 - age) * 18, 240) : 0
        let tipY = 172 + dip
        screen.drawLine(x, 182, x + 19, tipY - 1, 15)
        screen.drawLine(x, 183, x + 19, tipY, 11)
        screen.drawLine(x, 184, x + 19, tipY + 1, 8)
        screen.fillRect(x + 17, tipY - 2, 6, 5, 14)
        screen.drawLine(x + 18, tipY - 2, x + 21, tipY - 2, 4)
        screen.fillCircle(x, 183, 2, 13)
        // Catch bucket below the spout; the produced FullBucket is still a
        // separate learner-facing pickup above the station.
        screen.drawTransparentImage(itemImage("water"), x - 21, 193)
        if (pumpStrokeValid && age >= 100 && age < 330) {
            screen.drawLine(x - 14, 188, x - 14, 198, 9)
            screen.drawLine(x - 13, 190, x - 13, 197, 1)
            screen.setPixel(x - 17, 197 - Math.idiv(age, 90) % 3, 9)
        }
    }

    function drawFencePlaque(label: string, left: number, top: number, width: number = 0) {
        if (width == 0) width = label.length * 6 + 10
        screen.fillRect(left, top, width, 13, 14)
        screen.fillRect(left + 1, top + 1, width - 2, 10, 4)
        screen.drawLine(left + 2, top + 1, left + width - 3, top + 1, 5)
        screen.print(label, left + 5, top + 3, 15)
        screen.setPixel(left + 2, top + 6, 11); screen.setPixel(left + width - 3, top + 6, 11)
    }

    function drawEnclosureSigns() {
        for (let slot = 0; slot < 3; slot++) {
            let x = slot * 106 + 4
            // Bolted directly onto the existing back rail, not a freestanding sign.
            drawFencePlaque(chosen[slot], x + 3, 24, 93)
            for (let i = 0; i < 3; i++) heart(x + 56 + i * 11, 27, reportedLove[slot] > i)
            let c = creatures[slot]
            if (c != null) {
                let name = reportedNames[slot].length > 0 ? reportedNames[slot] : "- - -"
                // Match the species plaque on the front-right fence rail.
                drawFencePlaque(name, x + 99 - (name.length * 6 + 10), 122)
            }
        }
    }

    function showEnergyGain(amount: number) {
        let text = "+" + amount
        let small = image.create(text.length * 6, 8)
        small.print(text, 0, 0, 5)
        let large = image.create(small.width * 2 + 4, 20)
        for (let y = 0; y < 8; y++) for (let x = 0; x < small.width; x++) {
            if (small.getPixel(x, y) != 0) large.fillRect(x * 2 + 1, y * 2 + 1, 4, 4, 15)
        }
        for (let y = 0; y < 8; y++) for (let x = 0; x < small.width; x++) {
            if (small.getPixel(x, y) != 0) large.fillRect(x * 2 + 2, y * 2 + 2, 2, 2, 5)
        }
        if (energyGainImages.length >= 6) {
            energyGainImages.shift(); energyGainX.shift(); energyGainY.shift(); energyGainAt.shift()
        }
        energyGainImages.push(large)
        energyGainX.push(Math.max(2, Math.min(318 - large.width, Math.round(ranger.x) - Math.idiv(large.width, 2))))
        energyGainY.push(Math.round(ranger.y) - 30)
        energyGainAt.push(control.millis())
    }

    function drawEnergyGains() {
        while (energyGainAt.length > 0 && control.millis() - energyGainAt[0] >= 1300) {
            energyGainImages.shift(); energyGainX.shift(); energyGainY.shift(); energyGainAt.shift()
        }
        for (let i = 0; i < energyGainImages.length; i++) {
            let age = control.millis() - energyGainAt[i]
            screen.drawTransparentImage(energyGainImages[i], energyGainX[i], Math.max(25, energyGainY[i] - Math.idiv(age, 55)))
        }
    }

    function announce(text: string, duration: number = 1800) {
        statusText = text
        statusUntil = control.millis() + duration
    }

    function nearXY(x: number, y: number, distance: number): boolean {
        return ranger != null && Math.abs(ranger.x - x) <= distance && Math.abs(ranger.y - y) <= distance
    }

    function nearestStation(): number {
        let selected = -1
        let distance = 1000
        for (let i = 0; i < 4; i++) {
            if (nearXY(stationX[i], 198, 31) && Math.abs(ranger.x - stationX[i]) < distance) {
                selected = i; distance = Math.abs(ranger.x - stationX[i])
            }
        }
        return selected
    }

    function stationOpen(index: number): boolean {
        return index == 3 ? unlocked > 0 : index >= 0 && index < unlocked
    }

    function pickup(index: number) {
        // Only preparation is supplied. Collection and destruction belong to the learner.
        if (sprites.allOfKind(ingredientKinds[index]).length > 0) {
            announce("Collect the serving above the bin")
            return
        }
        let item = sprites.create(itemImage(words[index]), ingredientKinds[index])
        item.setPosition(stationX[index], 165); item.z = 10
        announce("Ready! Walk up to collect it")
        console.log("FCI prepared=" + words[index])
    }

    function setupSnack(index: number) {
        if (index >= unlocked || sprites.allOfKind(snackKinds[index]).length > 0) return
        if (control.millis() < snackReadyAt[index]) return
        // Let the ranger leave before a replacement snack appears. Collection
        // and the energy change still belong to the learner's overlap event.
        if (nearXY(snackX[index], snackY, 24)) return
        let item = sprites.create(itemImage(words[index + 4]), snackKinds[index])
        item.setPosition(snackX[index], snackY); item.z = 10
        console.log("FCI snack-ready=" + index + " at=" + control.millis())
    }

    function snackCollected(index: number) {
        snackReadyAt[index] = control.millis() + snackCooldownMs[index]
        console.log("FCI snack-collected=" + index + " at=" + control.millis() + " until=" + snackReadyAt[index])
    }

    function setupTrough(slot: number, kind: number) {
        let p = image.create(18, 34)
        p.fillRect(0, 1, 18, 32, 14)
        p.fillRect(1, 1, 16, 30, 4)
        p.drawRect(1, 0, 16, 30, 5); p.fillRect(3, 3, 12, 24, 14)
        p.drawLine(1, 31, 16, 31, 14)
        p.drawLine(1, 8, 2, 8, 1); p.drawLine(15, 23, 16, 23, 1)
        let trough = sprites.create(p, kind)
        trough.setPosition(troughX[slot], 90); trough.z = 3
    }

    function admit(slot: number, value: string, kind: number, body: number, accent: number, mark: string) {
        if (value != chosen[slot] || admitted[slot]) return
        // The learner's display block is the causal arrival action. Build the
        // supplied world first if needed, then create the chosen creature in
        // this same call—there is no deferred request that can be lost across
        // a tutorial compile or simulator restart.
        if (!worldStarted) startWorld()
        admitted[slot] = true
        let creature = sprites.create(creatureImage(body, accent, mark), kind)
        for (let blink = 0; blink < 2; blink++) for (let phase = 0; phase < 4; phase++) {
            creatureFrames[slot].push(creatureFrame(creature.image, mark, phase, blink == 1))
        }
        creature.setPosition(homeX[slot], 78); creature.z = 5
        creatures[slot] = creature
        orderReady[slot] = true
        creatureKinds[slot] = kind
        unlocked = Math.max(unlocked, slot + 1)
        setupSnack(slot)
        announce(chosen[slot] + " has arrived!")
        console.log("FCI arrival=" + chosen[slot])
    }

    function showName(slot: number, value: string) {
        reportedNames[slot] = value
        if (creatures[slot] != null && value.length > 0) announce(chosen[slot] + " is now " + value + "!", 6000)
        console.log("ANIMAL_CARE name slot=" + (slot + 1) + " value=" + value)
    }

    function showLove(slot: number, value: number) {
        let previous = reportedLove[slot]
        reportedLove[slot] = value
        if (value > previous) {
            affectionAt[slot] = control.millis()
            announce(reportedNames[slot] + " enjoys the petting!")
        }
        console.log("ANIMAL_CARE love slot=" + (slot + 1) + " value=" + value)
    }

    function showWater(slot: number, value: number) {
        let previous = reportedWater[slot]
        reportedWater[slot] = value
        if (value > previous) {
            waterAt[slot] = control.millis()
            nextDrink[slot] = control.millis() + 1300
            announce(chosen[slot] + " water +" + (value - previous))
        } else if (value < previous && drinking[slot]) {
            drank[slot] = true; drinking[slot] = false; returning[slot] = true
            // The first learner-authored drink change ends this contact. The
            // creature keeps its appearance, but its temporary kind prevents
            // the overlap event from subtracting water again every frame.
            creatures[slot].setKind(SpriteKind.Food)
            creatures[slot].setFlag(SpriteFlag.GhostThroughSprites, true)
            nextDrink[slot] = control.millis() + 12000
            announce(chosen[slot] + " drinks " + (previous - value))
            console.log("FCI drank=" + slot + " amount=" + (previous - value))
        }
        console.log("ANIMAL_CARE water slot=" + (slot + 1) + " value=" + value)
    }

    function moveCreature(slot: number, x: number, y: number, speed: number = 32): boolean {
        let c = creatures[slot]
        c.vx = Math.abs(c.x - x) < 2 ? 0 : c.x < x ? speed : -speed
        c.vy = Math.abs(c.y - y) < 2 ? 0 : c.y < y ? speed : -speed
        return c.vx == 0 && c.vy == 0
    }

    function nudgeRanger(dx: number, dy: number) {
        // Continuous movement still comes from controller.moveSprite. A small
        // immediate nudge also makes ordinary taps visible and dependable.
        if (ranger == null) return
        if (energyShown && reportedEnergy <= 0) { dx *= 0.4; dy *= 0.4 }
        ranger.x += dx
        ranger.y += dy
        console.log("FCI nudge dx=" + dx + " dy=" + dy)
    }

    function trackWalking() {
        let dx = ranger.x - lastRangerX, dy = ranger.y - lastRangerY
        let distance = Math.sqrt(dx * dx + dy * dy)
        lastRangerX = ranger.x; lastRangerY = ranger.y
        if (distance <= 0.01) return
        movingUntil = control.millis() + 180
        if (!energyShown || walkingHandler == null) return
        walkingDistance += distance
        while (walkingDistance >= 45) {
            walkingDistance -= 45
            console.log("FCI walk-step at=" + control.millis() + " energy=" + reportedEnergy)
            // The learner handler, not the world, decides how energy changes.
            walkingHandler()
        }
    }

    function nearestPettable(): number {
        for (let slot = 0; slot < 3; slot++) {
            let c = creatures[slot]
            if (c != null && !drinking[slot] && !returning[slot] && nearXY(c.x, c.y, 24)) return slot
        }
        return -1
    }

    function petStroke(button: number): boolean {
        let slot = nearestPettable()
        if (slot < 0 || reportedPlate.length > 0) { petStrokes = 0; petSlot = -1; return false }
        let now = control.millis()
        if (now < petReadyAt) return true
        if (slot != petSlot || now - lastPetAt > 1800) petStrokes = 0
        petSlot = slot
        let expected = petStrokes % 2 == 0 ? 5 : 6
        if (button != expected || (petStrokes > 0 && now - lastPetAt < 200)) {
            petStrokes = 0
            announce("Pet gently: A B A B")
            return true
        }
        petStrokes += 1; lastPetAt = now
        announce("PET: " + (petStrokes % 2 == 0 ? "A next" : "B next"), 900)
        if (petStrokes == 4) {
            petStrokes = 0; petReadyAt = now + 1200
            console.log("FCI pet-gesture=" + slot + " at=" + now)
            if (petHandlers[slot] != null) petHandlers[slot]()
        }
        return true
    }

    function plateMatchesOrder(slot: number, value: string[]): boolean {
        if (!orderReady[slot] || value.length == 0 || value.length != orders[slot].length) return false
        for (let i = 0; i < value.length; i++) if (value[i] != orders[slot][i]) return false
        return true
    }

    function ready(): boolean {
        for (let slot = 0; slot < 3; slot++) {
            if (creatures[slot] == null || reportedNames[slot].length == 0 || reportedLove[slot] < 1 || !drank[slot] || meals[slot] < 1) return false
        }
        return ateEnergyFood && energyDecayed && reportedPlate.length == 0
    }

    function heart(x: number, y: number, filled: boolean) {
        let color = filled ? 2 : 11
        screen.fillRect(x + 1, y, 2, 2, color); screen.fillRect(x + 5, y, 2, 2, color)
        screen.fillRect(x, y + 2, 8, 2, color); screen.fillRect(x + 1, y + 4, 6, 1, color)
        screen.fillRect(x + 2, y + 5, 4, 1, color); screen.fillRect(x + 3, y + 6, 2, 1, color)
    }

    function drawOrder(slot: number, x: number) {
        if (creatures[slot] == null) return
        let c = creatures[slot]
        let top = Math.max(39, Math.round(c.y) - 34)
        if (control.millis() < servedUntil[slot]) {
            screen.print("YUM!", Math.round(c.x) - 12, top + 5, 15)
            heart(Math.round(c.x) + 15, top + 4, true)
            return
        }
        if (!orderVisible[slot]) return
        let recipe = orders[slot]
        let width = recipe.length * 15 + 8
        let left = Math.max(x + 3, Math.min(x + 96 - width, Math.round(c.x) - Math.idiv(width, 2)))
        // A small plate-shaped thought, preserving exact left-to-right portions.
        oval(screen, left, top + 2, width, 18, 11)
        oval(screen, left, top, width, 18, 1)
        oval(screen, left + 2, top + 2, width - 4, 13, 13)
        for (let i = 0; i < recipe.length; i++) screen.drawTransparentImage(itemImage(recipe[i]), left + 4 + i * 15, top)
        screen.fillCircle(Math.round(c.x) + 6, top + 22, 2, 1)
        screen.setPixel(Math.round(c.x) + 3, top + 26, 1)
    }

    function updateOrders() {
        let now = control.millis()
        for (let slot = 0; slot < 3; slot++) {
            if (creatures[slot] == null) continue
            if (!orderReady[slot] && now >= nextMealAt[slot]) {
                nextOrder(slot)
                orderReady[slot] = true
            }
            // A pending order stays visible until it is successfully served.
            let visible = orderReady[slot]
            if (visible != orderVisible[slot]) {
                orderVisible[slot] = visible
                console.log("FCI order-" + (visible ? "visible=" : "hidden=") + slot + " at=" + now + " recipe=" + orders[slot].join(","))
            }
            let matching = plateMatchesOrder(slot, reportedPlate)
            if (matching != plateMatchShown[slot]) {
                plateMatchShown[slot] = matching
                console.log("FCI plate-pulse=" + slot + " matching=" + matching + " at=" + now)
            }
        }
    }

    function nextOrder(slot: number) {
        // Relative weights: 30 one-portion, 50 two-portion, 25 three-portion.
        // First teaching meals are declared above; only later meals are random.
        let roll = randint(1, 105)
        let count = roll <= 30 ? 1 : roll <= 80 ? 2 : 3
        let available = Math.max(1, Math.min(unlocked, knownIngredients))
        let recipe: string[] = []
        // Independent draws allow repeated portions and any eligible combination.
        for (let i = 0; i < count; i++) recipe.push(words[randint(0, available - 1)])
        orders[slot] = recipe
        console.log("FCI next-order=" + slot + " recipe=" + recipe.join(","))
    }

    function drawHud() {
        let message = statusText
        if (control.millis() > statusUntil) {
            let station = nearestStation()
            if (shiftWon) message = "FIRST SHIFT COMPLETE! Keep caring!"
            else if (nearestPettable() >= 0 && reportedPlate.length == 0) message = "PET: A B A B (empty hands)"
            else if (station >= 0 && !stationOpen(station)) message = "This station opens with its creature"
            else if (station == 0) message = "SEEDS: press A once"
            else if (station == 1) message = "BERRIES: hold A until ready"
            else if (station == 2) message = "GREENS: tap A three times"
            else if (station == 3) message = "PUMP: A ... A ... A (steady beats)"
            else message = "Arrows: walk   A: prepare   B: offer plate"
        }
        screen.print(message, Math.max(3, Math.idiv(320 - message.length * 6, 2)), 7, shiftWon ? 5 : 1)
        for (let slot = 0; slot < 3; slot++) {
            let x = slot * 106 + 4
            drawOrder(slot, x)
            let c = creatures[slot]
            if (plateMatchesOrder(slot, reportedPlate)) {
                let pulse = Math.idiv(control.millis(), 350) % 2 == 0 ? 5 : 9
                oval(screen, x + 17, 111, 44, 12, pulse)
                oval(screen, x + 21, 114, 36, 6, 1)
                screen.drawLine(x + 16, 108, x + 13, 105, pulse)
                screen.drawLine(x + 63, 108, x + 66, 105, pulse)
            }
            let height = Math.idiv(Math.max(0, Math.min(20, reportedWater[slot])) * 24, 20)
            screen.fillRect(troughX[slot] - 6, 100 - height, 12, height, 9)
            if (height > 3) {
                let ripple = Math.idiv(control.millis(), 220) % (height - 2)
                screen.drawLine(troughX[slot] - 3, 99 - ripple, troughX[slot] + 3, 99 - ripple, 1)
            }
            screen.fillRect(troughX[slot] - 8, 112, 3, 3, 9)
            screen.setPixel(troughX[slot] - 7, 111, 9)
            screen.print("" + reportedWater[slot], troughX[slot] - 3, 110, 15)
            if (reportedWater[slot] <= 0 && c != null) {
                let warning = Math.idiv(control.millis(), 900) % 2 == 0 ? 2 : 5
                screen.drawRect(troughX[slot] - 9, 73, 18, 31, warning)
                screen.print("EMPTY", troughX[slot] - 16, 64, warning)
            }
            let splashAge = control.millis() - waterAt[slot]
            if (splashAge < 650) {
                let lift = Math.idiv(splashAge, 120)
                screen.fillRect(troughX[slot] - 5, 76 - lift, 2, 2, 9)
                screen.fillRect(troughX[slot] + 4, 74 - lift, 2, 2, 9)
            }
            let loveAge = control.millis() - affectionAt[slot]
            if (c != null && loveAge < 1200) heart(Math.round(c.x) + 12, Math.round(c.y) - 15 - Math.idiv(loveAge, 120), true)
        }
        let labels = ["SEEDS", "BERRY", "GREENS", "PUMP"]
        for (let i = 0; i < 4; i++) {
            screen.print(labels[i], stationX[i] - labels[i].length * 3, 211, 15)
            if (!stationOpen(i)) {
                // A tiny padlock marks availability without hiding the object.
                screen.drawRect(stationX[i] - 3, 197, 6, 5, 15)
                screen.fillRect(stationX[i] - 4, 200, 8, 6, 11)
                screen.setPixel(stationX[i], 203, 15)
            }
        }
        let progress = [0, berryHoldAt == 0 ? 0 : Math.min(3, Math.idiv(control.millis() - berryHoldAt, 220) + 1), greensTaps, pumpBeats]
        for (let i = 1; i < 4; i++) {
            if (stationOpen(i)) for (let j = 0; j < 3; j++) screen.fillRect(stationX[i] - 12 + j * 9, 207, 7, 2, j < progress[i] ? 9 : 14)
        }
        if (nearestStation() == 3 && lastPumpBeatAt > 0) {
            let age = control.millis() - lastPumpBeatAt
            screen.fillCircle(188, 203, 2, age >= 320 ? 9 : 2)
        }
        screen.print("PLATE", 5, 226, 1)
        for (let i = 0; i < 3; i++) {
            screen.drawRect(42 + i * 19, 221, 17, 17, 11)
            if (i < reportedPlate.length) screen.drawTransparentImage(itemImage(reportedPlate[i]), 43 + i * 19, 222)
        }
        if (reportedPlate.length > 3) screen.print("+" + (reportedPlate.length - 3), 101, 226, 3)
        screen.drawTransparentImage(itemImage("water"), 121, 222)
        screen.print("" + reportedBucket, 141, 226, 9)
        let exhaustedMoving = energyShown && reportedEnergy <= 0 && control.millis() < movingUntil
        let energyColor = exhaustedMoving && Math.idiv(control.millis(), 250) % 2 == 0 ? 2 : 1
        screen.print("ENERGY " + reportedEnergy, 181, 226, energyColor)
        screen.drawRect(261, 226, 53, 7, exhaustedMoving ? energyColor : 11)
        screen.fillRect(262, 227, Math.idiv(Math.max(0, Math.min(100, reportedEnergy)) * 51, 100), 5, 7)
        drawEnergyGains()
        if (shiftWon) {
            for (let i = 0; i < 18; i++) {
                let y = (Math.idiv(control.millis(), 40) + i * 11) % 108 + 25
                screen.fillRect((i * 43 + 17) % 318, y, 2, 3, 2 + i % 8)
            }
        }
    }

    controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
        if (petStroke(5)) return
        let selected = nearestStation()
        if (!stationOpen(selected)) return
        if (selected == 0) pickup(0)
        else if (selected == 2) {
            if (control.millis() - lastGreenTapAt > 1400) greensTaps = 0
            greensTaps += 1; lastGreenTapAt = control.millis()
            if (greensTaps >= 3) { greensTaps = 0; pickup(2) }
        } else if (selected == 3) {
            let now = control.millis()
            pumpStrokeAt = now
            pumpStrokeValid = lastPumpBeatAt == 0 || now - lastPumpBeatAt >= 320
            if (lastPumpBeatAt == 0 || now - lastPumpBeatAt >= 320) pumpBeats += 1
            else { pumpBeats = 1; announce("Steady beats, not fast taps") }
            lastPumpBeatAt = now
            if (pumpBeats >= 3) { pumpBeats = 0; lastPumpBeatAt = 0; pickup(3) }
        }
    })

    // System listener coexists with the learner's B offering event.
    controller.B.addEventListener(ControllerButtonEvent.Pressed, function () { petStroke(6) })

    controller.left.onEvent(ControllerButtonEvent.Pressed, function () { nudgeRanger(-6, 0) })
    controller.right.onEvent(ControllerButtonEvent.Pressed, function () { nudgeRanger(6, 0) })
    controller.up.onEvent(ControllerButtonEvent.Pressed, function () { nudgeRanger(0, -6) })
    controller.down.onEvent(ControllerButtonEvent.Pressed, function () { nudgeRanger(0, 6) })

    controller.A.onEvent(ControllerButtonEvent.Released, function () {
        berryHoldAt = 0; berryPrepared = false
    })

    game.onUpdate(function () {
        // An empty starter still receives its supplied ranger and habitats on
        // the first update. If the learner admits a creature first, admit()
        // has already initialized this same world synchronously.
        if (!worldStarted) startWorld()
        if (ranger == null) return
        ranger.y = Math.max(36, Math.min(210, ranger.y))
        trackWalking()
        if (petStrokes > 0 && (nearestPettable() != petSlot || reportedPlate.length > 0 || control.millis() - lastPetAt > 1800)) {
            petStrokes = 0; petSlot = -1
        }
        if (!controller.A.isPressed() || nearestStation() != 1 || !stationOpen(1)) {
            berryHoldAt = 0; berryPrepared = false
        } else if (!berryPrepared) {
            if (berryHoldAt == 0) berryHoldAt = control.millis()
            else if (control.millis() - berryHoldAt >= 650) { berryPrepared = true; pickup(1) }
        }
        if (control.millis() - lastGreenTapAt > 1400) greensTaps = 0
        updateOrders()
        for (let slot = 0; slot < 3; slot++) {
            let c = creatures[slot]
            if (c == null) continue
            if (returning[slot]) {
                if (moveCreature(slot, homeX[slot], 78)) {
                    returning[slot] = false
                    c.setKind(creatureKinds[slot])
                    c.setFlag(SpriteFlag.GhostThroughSprites, false)
                }
            } else if (drinking[slot]) moveCreature(slot, troughX[slot], 86)
            else if (!shiftWon && reportedWater[slot] >= costs[slot] && control.millis() >= nextDrink[slot]) {
                drinking[slot] = true; moveCreature(slot, troughX[slot], 86)
            } else if (nearXY(c.x, c.y, 46) && Math.abs(ranger.x - homeX[slot]) <= 34 && Math.abs(ranger.x - troughX[slot]) > 28 && ranger.y < 132) {
                // A nearby creature eagerly closes the last small gap. The
                // learner still owns the pet event and love change; approach
                // alone earns nothing. Stop nearby for intentional A/B petting.
                // The explicit trough exclusion keeps it out of an unscheduled
                // drink even if the ranger stops a few pixels off center.
                moveCreature(slot, Math.min(ranger.x, homeX[slot] + 6), ranger.y, 42)
            } else if (!nearXY(c.x, c.y, 35)) {
                // Tiny unhurried strolls stay near the petting area. Approaching
                // the creature stops wandering so it never evades a learner.
                let wander = Math.idiv(control.millis() + slot * 1700, 3500) % 3
                moveCreature(slot, homeX[slot] + (wander == 0 ? -5 : wander == 1 ? 6 : 0), wander == 1 ? 82 : 78, 9)
            } else {
                c.vx = 0; c.vy = 0
            }
        }
        if (!shiftWon && ready()) {
            shiftWon = true
            console.log("FCI first-shift=complete")
        }
    })

    game.onUpdateInterval(200, function () {
        for (let i = 0; i < 3; i++) setupSnack(i)
    })
    game.onUpdateInterval(120, function () {
        if (ranger == null || rangerFrames.length == 0) return
        let moving = Math.abs(ranger.vx) > 1 || Math.abs(ranger.vy) > 1
        if (Math.abs(ranger.vx) > 1) rangerFacing = ranger.vx < 0 ? 2 : 3
        else if (Math.abs(ranger.vy) > 1) rangerFacing = ranger.vy < 0 ? 1 : 0
        ranger.setImage(rangerFrames[rangerFacing * 4 + (moving ? Math.idiv(control.millis(), 120) % 4 : 0)])
        for (let slot = 0; slot < 3; slot++) {
            if (creatures[slot] == null || creatureFrames[slot].length == 0) continue
            let time = control.millis() + slot * 430
            let phase = Math.idiv(time, 260) % 4
            let blink = time % 4200 > 3950 ? 4 : 0
            creatures[slot].setImage(creatureFrames[slot][phase + blink])
        }
    })
    game.onPaint(function () { if (worldStarted) drawPump() })
    // Signs are above trough art (3), below animals (5) and ranger (12).
    // This keeps long learner names visible without making signs an overlay.
    scene.createRenderable(4, function () { if (worldStarted) drawEnclosureSigns() })
    game.onShade(function () { if (worldStarted) drawHud() })

    //% blockHidden=true
    export function startWorld() {
        if (worldStarted) return
        worldStarted = true
        // Main declares the learner-visible kinds after customts is loaded.
        // Resolve these identities on first use, never during namespace init.
        ingredientKinds = [SpriteKind.Seeds, SpriteKind.Berries, SpriteKind.Greens, SpriteKind.FullBucket]
        snackKinds = [SpriteKind.Apple, SpriteKind.Sandwich, SpriteKind.Cake]
        sprites.onDestroyed(SpriteKind.Apple, function () { snackCollected(0) })
        sprites.onDestroyed(SpriteKind.Sandwich, function () { snackCollected(1) })
        sprites.onDestroyed(SpriteKind.Cake, function () { snackCollected(2) })
        image.setPalette(hex`000000fff5dfe47c81f3a6bfeab46bf5dd9470a78badd49b547aa994d9dc9983bcafadb8715a70f4e6cf76564f35434e`)
        scene.setBackgroundImage(makeBackground())
        for (let direction = 0; direction < 4; direction++) for (let phase = 0; phase < 4; phase++) {
            rangerFrames.push(walkingFrame(direction, phase))
        }
        ranger = sprites.create(rangerImage(), SpriteKind.Player)
        ranger.setPosition(160, 155); ranger.z = 12; ranger.setStayInScreen(true)
        lastRangerX = ranger.x; lastRangerY = ranger.y
        controller.moveSprite(ranger, 90, 90)
        setupTrough(0, SpriteKind.DragonTrough)
        setupTrough(1, SpriteKind.UnicornTrough)
        setupTrough(2, SpriteKind.PhoenixTrough)
        console.log("FCI world=ready resolution=320x240")
    }

    //% block="show $value in the 1st enclosure"
    export function showAnimal1(value: string) { admit(0, value, SpriteKind.Dragon, 2, 4, "wings") }
    //% block="show $value in the 2nd enclosure"
    export function showAnimal2(value: string) { admit(1, value, SpriteKind.Unicorn, 13, 5, "horn") }
    //% block="show $value in the 3rd enclosure"
    export function showAnimal3(value: string) { admit(2, value, SpriteKind.Phoenix, 4, 2, "flame") }

    //% block="show $value beside Dragon"
    export function showDragonName(value: string) { showName(0, value) }
    //% block="show $value beside Unicorn"
    export function showUnicornName(value: string) { showName(1, value) }
    //% block="show $value beside Phoenix"
    export function showPhoenixName(value: string) { showName(2, value) }
    //% block="show $value on Dragon's love meter"
    export function showDragonLove(value: number) { showLove(0, value) }
    //% block="show $value on Unicorn's love meter"
    export function showUnicornLove(value: number) { showLove(1, value) }
    //% block="show $value on Phoenix's love meter"
    export function showPhoenixLove(value: number) { showLove(2, value) }

    //% block="on Dragon petted"
    export function onDragonPetted(handler: () => void) { petHandlers[0] = handler }
    //% block="on Unicorn petted"
    export function onUnicornPetted(handler: () => void) { petHandlers[1] = handler }
    //% block="on Phoenix petted"
    export function onPhoenixPetted(handler: () => void) { petHandlers[2] = handler }
    //% block="on ranger walking"
    export function onRangerWalk(handler: () => void) { walkingHandler = handler }
    //% block="show $value on Dragon's water meter"
    export function showDragonWater(value: number) { showWater(0, value) }
    //% block="show $value on Unicorn's water meter"
    export function showUnicornWater(value: number) { showWater(1, value) }
    //% block="show $value on Phoenix's water meter"
    export function showPhoenixWater(value: number) { showWater(2, value) }

    //% block="show $value on the plate"
    export function showPlate(value: string[]) {
        // Copy for display; never append to, clear, or otherwise mutate the learner's list.
        reportedPlate = []
        for (let item of value) reportedPlate.push(item)
        if (reportedPlate.length > 0) { petStrokes = 0; petSlot = -1 }
        for (let item of value) {
            for (let i = 0; i < 3; i++) if (item == words[i]) knownIngredients = Math.max(knownIngredients, i + 1)
        }
        console.log("ANIMAL_CARE plate=" + reportedPlate.join(","))
    }

    //% block="offer $value to the creature here"
    export function servePlate(value: string[]) {
        if (ranger == null) return
        // B is also a petting stroke with empty hands. Offering nothing is quiet.
        if (value.length == 0) return
        for (let slot = 0; slot < 3; slot++) {
            if (creatures[slot] != null && ranger.y < 156 && ranger.x >= slot * 106 && ranger.x < (slot + 1) * 106) {
                if (!orderReady[slot]) {
                    announce(chosen[slot] + ": YUM! THANKS!")
                    console.log("FCI meal-rest=" + slot + " at=" + control.millis())
                    return
                }
                let correct = plateMatchesOrder(slot, value) && plateMatchesOrder(slot, reportedPlate)
                if (correct) {
                    meals[slot] += 1
                    servedUntil[slot] = control.millis() + 2200
                    nextMealAt[slot] = control.millis() + mealRestMs
                    orderReady[slot] = false
                    orders[slot] = []
                    announce(chosen[slot] + ": meal accepted!")
                    console.log("FCI meal=" + slot + " order=" + value.join(","))
                    console.log("FCI meal-cooldown=" + slot + " until=" + nextMealAt[slot] + " at=" + control.millis())
                } else {
                    announce("Not that order. Try a fresh plate.")
                    console.log("FCI rejected=" + slot + " order=" + value.join(","))
                }
                return
            }
        }
        announce("Offer meals inside an enclosure")
    }

    //% block="show $value in the bucket"
    export function showBucket(value: number) {
        reportedBucket = value
        console.log("ANIMAL_CARE bucket=" + value)
    }
    //% block="use $value for the ranger's energy meter and speed"
    export function useEnergy(value: number) {
        if (energyShown && value > reportedEnergy) {
            ateEnergyFood = true
            if (ranger != null) showEnergyGain(value - reportedEnergy)
        }
        if (energyShown && value < reportedEnergy) energyDecayed = true
        reportedEnergy = value; energyShown = true
        if (ranger != null) {
            let speed = value > 0 ? 90 : 36
            controller.moveSprite(ranger, speed, speed)
        }
        console.log("ANIMAL_CARE energy=" + value)
    }
}
```
