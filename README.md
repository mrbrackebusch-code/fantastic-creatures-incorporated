# Fantastic Creatures Incorporated

### @explicitHints true

## Welcome, ranger!

Hello ranger! Welcome to your first day on the job at Fantastic Creatures Incorporated! We plan on placing 3 animals into your care today.

Each animal needs food, water, and love.

To keep track of all the different things each animal needs, we will need ``||variables:Variables||``.

``||variables:Variables||`` are simply **containers that we can store values inside**. ``||variables:Variables||`` can hold anything, and today you will store numbers, words, and lists in them as you take care of your animals.

``||variables:Variables||`` can be ``||variables:set||`` (where we *erase* what was inside before and *replace* it) or ``||variables:changed||`` (where we *add* or *remove* something from the ``||variables:variable||`` but leave the rest alone).

To start let's update the ``||variables:variable||`` for your 1st creature!

## 1. Bring in Dragon

Your 1st enclosure is ready for Dragon. The game needs somewhere to keep that choice.

### What to do

**Make a ``||variables:variable||`` to remember your 1st creature.**

### Add this code

- [ ] Open ``||variables:Variables||``.

- [ ] Make a new ``||variables:variable||`` named ``||variables:animal1||``.

- [ ] From ``||loops:Loops||``, drag an ``||loops:on start||`` block into the workspace.

- [ ] From ``||variables:Variables||``, place ``||variables:set animal1 to||`` inside ``||loops:on start||``.

- [ ] Open **Advanced** → ``||text:Text||``.

- [ ] Put the ``||text:" "||`` word block into ``||variables:set animal1 to||``.

- [ ] Type ``||text:Dragon||`` between its quotes.

- [ ] From ``||animalCare:Care Displays||``, add ``||animalCare:show value in the 1st enclosure||`` under the set block.

- [ ] Put ``||variables:animal1||`` into that show block.

### What you should see

- [ ] Run your game.

- [ ] Click the game screen.

- [ ] Use the arrow keys to walk around.

Your Dragon should appear in the 1st enclosure.

**Keyboard controls:** **Space** is the **A** button. **Enter** is the **B** button.

![first arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/01-first-arrival.gif)

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
    export const Soup = SpriteKind.create()
}

let animal1 = ""

animal1 = "Dragon"

animalCare.showAnimal1(animal1)
```

## 2. Name Dragon

Your Dragon needs a name.

### What to do

**Make a ``||variables:variable||`` to remember your Dragon's name.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:dragonName||``.

- [ ] Pick one name: `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] In ``||loops:on start||``, place ``||variables:set dragonName to||`` under the block that shows ``||variables:animal1||`` in the 1st enclosure.

- [ ] Put the ``||text:" "||`` word block from **Advanced** → ``||text:Text||`` into the set block.

- [ ] Type the name you chose between its quotes.

- [ ] From ``||animalCare:Care Displays||``, add ``||animalCare:show value beside Dragon||`` under the set block.

- [ ] Put ``||variables:dragonName||`` into that show block.

### What you should see

- [ ] Run your game.

A dark name tag should keep showing your chosen word beside Dragon. A message at the top should briefly welcome Dragon by that name.

![first name: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/02-first-name.gif)

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
    export const Soup = SpriteKind.create()
}

let dragonName = ""

dragonName = "Pip"

animalCare.showDragonName(dragonName)
```

## 3. Give Dragon love

Your Dragon's heart meter is empty. Walking over to your creature is how you give it love.

In the overlap blocks, the ranger is a sprite of kind ``||sprites:Player||``. Your first creature is kind ``||sprites:Dragon||``.

### What to do

**Make a ``||variables:variable||`` to remember how much love your Dragon has.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:dragonLove||``.

- [ ] From ``||sprites:Sprites||``, add an ``||sprites:overlap event||`` for a sprite of kind ``||sprites:Player||`` and a sprite of kind ``||sprites:Dragon||``.

- [ ] Inside the event, place ``||variables:change dragonLove by 1||`` from ``||variables:Variables||``.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:dragonLove||`` on Dragon's love meter inside the same event.

### What you should see

- [ ] Run your game.

- [ ] Walk over to your Dragon.

One heart should fill.

![first love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/03-first-love.gif)

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
    export const Soup = SpriteKind.create()
}

let dragonLove = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Dragon, function (sprite, otherSprite) {
    dragonLove += 1
    animalCare.showDragonLove(dragonLove)
})
```

## 4. Start the plate

Your Dragon ordered one serving of seeds. The plate needs to keep each ingredient in the order you collect it.

### What to do

**Make a ``||variables:variable||`` to remember what's on the plate.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:plate||``.

- [ ] Inside ``||loops:on start||``, place ``||variables:set plate to||``.

- [ ] Put the ``||arrays:empty array||`` block from **Advanced** → ``||arrays:Arrays||`` into the set block.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:plate||`` on the plate under the set block.

- [ ] Add an ``||sprites:overlap event||`` for a sprite of kind ``||sprites:Player||`` and a sprite of kind ``||sprites:Seeds||``.

- [ ] From **Advanced** → ``||arrays:Arrays||``, put ``||arrays:list add value to end||`` inside the ``||sprites:overlap event||``.

- [ ] Choose ``||variables:plate||`` for its list.

- [ ] Put ``||text:"seeds"||`` in its value slot.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:plate||`` on the plate inside this event.

- [ ] From ``||sprites:Sprites||``, add a ``||sprites:destroy||`` block at the end of this event.

- [ ] Drag ``||sprites:otherSprite||`` from this ``||sprites:overlap event||``'s header into the destroy block.

### What you should see

- [ ] Run your game.

- [ ] Press **A** once at the seed bin.

- [ ] Collect the serving that appears.

Seeds should appear in the 1st spot on the plate.

![plate: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/04-plate.gif)

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
    export const Soup = SpriteKind.create()
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

- [ ] From ``||controller:Controller||``, add an ``||controller:on B button pressed||`` event.

- [ ] Inside it, use ``||animalCare:Care Displays||`` to offer ``||variables:plate||`` to the creature here.

- [ ] Under that, set ``||variables:plate||`` to an ``||arrays:empty array||``.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:plate||`` on the plate.

### What you should see

- [ ] Collect seeds.

- [ ] Walk into Dragon's enclosure.

- [ ] Press **B**.

Its thought cloud should thank you, your plate should empty, and then a new order should appear. A repeated ingredient picture means another trip for another portion.

Wrong order? **B** also empties that plate so you can try again. The creature's thought cloud will keep showing the same order.

![serve: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/05-serve.gif)

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
    export const Soup = SpriteKind.create()
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

**Make a ``||variables:variable||`` to remember how much water is in the bucket.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:bucketWater||``.

- [ ] Inside ``||loops:on start||``, set ``||variables:bucketWater||`` to `0`.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:bucketWater||`` in the bucket under the set block.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:FullBucket||``.

- [ ] Inside the event, change ``||variables:bucketWater||`` by `10`.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:bucketWater||`` in the bucket inside this event.

- [ ] From ``||sprites:Sprites||``, add a ``||sprites:destroy||`` block at the end of this event.

- [ ] Put ``||sprites:otherSprite||`` from this event's header into the destroy block.

### What you should see

- [ ] Run your game.

- [ ] At the pump, press **A** three times with a short pause between presses: **A … A … A**.

- [ ] Walk up to collect the full bucket.

Its outline turns blue when the next beat is ready. The carried-water meter should change from `0` to `10`.

![bucket: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/06-bucket.gif)

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
    export const Soup = SpriteKind.create()
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

**Make a ``||variables:variable||`` to remember your Dragon's water.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:dragonWater||``.

- [ ] Inside ``||loops:on start||``, set ``||variables:dragonWater||`` to `0`.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:dragonWater||`` on Dragon's water meter under the set block.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:DragonTrough||``.

- [ ] Inside that event, change ``||variables:dragonWater||`` by ``||variables:bucketWater||``.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:dragonWater||`` on Dragon's water meter.

- [ ] Then set ``||variables:bucketWater||`` to `0`.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:bucketWater||`` in the bucket.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Dragon||`` and ``||sprites:DragonTrough||``.

- [ ] Inside that event, change ``||variables:dragonWater||`` by `-7`.

- [ ] From ``||animalCare:Care Displays||``, show ``||variables:dragonWater||`` on Dragon's water meter.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Dragon's trough.

The bucket should empty, the trough should fill, and one drink should lower only this water meter.

![first water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/07-first-water.gif)

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
    export const Soup = SpriteKind.create()
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

Taking care of creatures is hard work. The ranger moves faster with more energy.

### What to do

**Make a ``||variables:variable||`` to remember the ranger's energy.**

### Add this code

- [ ] Make a new ``||variables:variable||`` named ``||variables:playerEnergy||``.

- [ ] Inside ``||loops:on start||``, set ``||variables:playerEnergy||`` to `20`.

- [ ] Under it, add ``||animalCare:use value for the ranger's energy meter and speed||`` from ``||animalCare:Care Displays||``.

- [ ] Put ``||variables:playerEnergy||`` into that block.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Apple||``.

- [ ] Inside the event, change ``||variables:playerEnergy||`` by `5`.

- [ ] Use ``||variables:playerEnergy||`` for the ranger's energy meter and speed with the same ``||animalCare:Care Displays||`` block.

- [ ] Destroy the apple that touched the player using this event's ``||sprites:otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect an apple.

The energy meter should rise by `5`, and the ranger should move faster.

![energy: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/08-energy.gif)

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
    export const Soup = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Apple, function (sprite, otherSprite) {
    playerEnergy += 5
    animalCare.useEnergy(playerEnergy)
    otherSprite.destroy()
})

playerEnergy = 20

animalCare.useEnergy(playerEnergy)
```

## 9. Energy goes down, too

The ranger uses energy while the shift is running. The snacks now have a job to do.

### What to do

**Change the energy a little at a time.**

### Add this code

- [ ] From ``||game:Game||``, add an ``||game:on game update every 500 ms||`` event.

- [ ] Change its interval to `8000` ms. That is eight seconds.

- [ ] Inside the event, change ``||variables:playerEnergy||`` by `-1`.

- [ ] Use ``||variables:playerEnergy||`` for the ranger's energy meter and speed with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Watch the energy number for eight seconds.

- [ ] Collect an apple to add `5` back.

The first point is used when the shift starts: `20` becomes `19`. Eight seconds later, it becomes `18`. You can always keep walking, even when energy is low.

![energy timer: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/09-energy-timer.gif)

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
    export const Soup = SpriteKind.create()
}

let playerEnergy = 0

game.onUpdateInterval(8000, function () {
    playerEnergy += -1
    animalCare.useEnergy(playerEnergy)
})
```

## 10. Bring in Unicorn

Your 2nd enclosure is ready for Unicorn.

### What to do

**Make a ``||variables:variable||`` to remember your 2nd creature.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:animal2||``.

- [ ] Set ``||variables:animal2||`` to ``||text:"Unicorn"||`` in ``||loops:on start||``.

- [ ] Show ``||variables:animal2||`` in the 2nd enclosure with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

Unicorn should enter the 2nd enclosure without replacing Dragon.

![second arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/10-second-arrival.gif)

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
    export const Soup = SpriteKind.create()
}

let animal2 = ""

animal2 = "Unicorn"

animalCare.showAnimal2(animal2)
```

## 11. Name and love Unicorn

Your new arrival needs its own name and its own hearts.

### What to do

**Make a ``||variables:variable||`` to remember your Unicorn's name.**

**Make a ``||variables:variable||`` to remember how much love your Unicorn has.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:unicornName||``.

- [ ] In ``||loops:on start||``, under the block that shows ``||variables:animal2||`` in the 2nd enclosure, set ``||variables:unicornName||`` to `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] Show ``||variables:unicornName||`` beside Unicorn with ``||animalCare:Care Displays||``.

- [ ] Make a new ``||variables:variable||`` named ``||variables:unicornLove||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Unicorn||``.

- [ ] Inside it, change ``||variables:unicornLove||`` by `1`.

- [ ] Show ``||variables:unicornLove||`` on Unicorn's love meter with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Walk over to Unicorn.

The new name should stay with Unicorn, and one love contact should fill only its heart meter.

![second name love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/11-second-name-love.gif)

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
    export const Soup = SpriteKind.create()
}

let unicornName = ""
let unicornLove = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Unicorn, function (sprite, otherSprite) {
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

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Berries||``.

- [ ] Inside it, add ``||text:"berries"||`` to the end of ``||variables:plate||`` with ``||arrays:Arrays||``.

- [ ] Show ``||variables:plate||`` on the plate with ``||animalCare:Care Displays||``.

- [ ] Destroy the berries that were collected using this event's ``||sprites:otherSprite||``.

### What you should see

- [ ] Hold **A** at the berry station until the serving appears.

- [ ] Collect berries.

- [ ] Collect seeds next.

- [ ] Carry the plate into Unicorn's enclosure.

- [ ] Press **B**.

The plate should show berries, then seeds. Its thought cloud should thank you, then show another order.

![berries: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/12-berries.gif)

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
    export const Soup = SpriteKind.create()
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

**Make a ``||variables:variable||`` to remember your Unicorn's water.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:unicornWater||``.

- [ ] Set ``||variables:unicornWater||`` to `0` in ``||loops:on start||``.

- [ ] Show ``||variables:unicornWater||`` on Unicorn's water meter with ``||animalCare:Care Displays||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:UnicornTrough||``.

- [ ] Inside it, change ``||variables:unicornWater||`` by ``||variables:bucketWater||``.

- [ ] Show ``||variables:unicornWater||`` on Unicorn's water meter with ``||animalCare:Care Displays||``.

- [ ] Set ``||variables:bucketWater||`` to `0`.

- [ ] Show ``||variables:bucketWater||`` in the bucket with ``||animalCare:Care Displays||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Unicorn||`` and ``||sprites:UnicornTrough||``.

- [ ] Inside it, change ``||variables:unicornWater||`` by `-4`.

- [ ] Show ``||variables:unicornWater||`` on Unicorn's water meter with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Unicorn's trough.

Only Unicorn's water meter should move.

![second water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/13-second-water.gif)

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
    export const Soup = SpriteKind.create()
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

A sandwich gives the ranger more energy than an apple.

### What to do

**Make the sandwich add more energy.**

### Make this happen

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Sandwich||``.

- [ ] Inside it, change ``||variables:playerEnergy||`` by `10`.

- [ ] Use ``||variables:playerEnergy||`` for the ranger's energy meter and speed with ``||animalCare:Care Displays||``.

- [ ] Destroy the sandwich using this event's ``||sprites:otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect a sandwich.

- [ ] Compare the meter change with the apple's `5`.

The sandwich should add `10` energy.

![second creature: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/14-second-creature.gif)

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
    export const Soup = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Sandwich, function (sprite, otherSprite) {
    playerEnergy += 10
    animalCare.useEnergy(playerEnergy)
    otherSprite.destroy()
})
```

## 15. Bring in Phoenix

The last roster card shows Phoenix.

### What to do

**Make a ``||variables:variable||`` to remember your 3rd creature.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:animal3||``.

- [ ] Set ``||variables:animal3||`` to ``||text:"Phoenix"||`` in ``||loops:on start||``.

- [ ] Show ``||variables:animal3||`` in the 3rd enclosure with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

All three creatures should now have their own enclosure.

![third arrival: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/15-third-arrival.gif)

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
    export const Soup = SpriteKind.create()
}

let animal3 = ""

animal3 = "Phoenix"

animalCare.showAnimal3(animal3)
```

## 16. Name and love Phoenix

Phoenix still needs a name and love of its own.

### What to do

**Make a ``||variables:variable||`` to remember your Phoenix's name.**

**Make a ``||variables:variable||`` to remember how much love your Phoenix has.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:phoenixName||``.

- [ ] In ``||loops:on start||``, under the block that shows ``||variables:animal3||`` in the 3rd enclosure, set ``||variables:phoenixName||`` to `Pip`, `Miso`, `Nori`, `Nova`, `Clover`, or `Pebble`.

- [ ] Show ``||variables:phoenixName||`` beside Phoenix with ``||animalCare:Care Displays||``.

- [ ] Make a new ``||variables:variable||`` named ``||variables:phoenixLove||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Phoenix||``.

- [ ] Inside it, change ``||variables:phoenixLove||`` by `1`.

- [ ] Show ``||variables:phoenixLove||`` on Phoenix's love meter with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Walk over to Phoenix.

The name and heart meter should belong to Phoenix.

![third name love: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/16-third-name-love.gif)

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
    export const Soup = SpriteKind.create()
}

let phoenixName = ""
let phoenixLove = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Phoenix, function (sprite, otherSprite) {
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

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Greens||``.

- [ ] Inside it, add ``||text:"greens"||`` to the end of ``||variables:plate||`` with ``||arrays:Arrays||``.

- [ ] Show ``||variables:plate||`` on the plate with ``||animalCare:Care Displays||``.

- [ ] Destroy the collected serving using this event's ``||sprites:otherSprite||``.

### What you should see

- [ ] Tap **A** three times at the greens station.

- [ ] Collect greens.

- [ ] Collect berries next.

- [ ] Collect seeds last.

- [ ] Check all three plate spots.

- [ ] Offer the finished plate to Phoenix with **B**.

The plate should keep greens, berries, then seeds in that order.

![greens: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/17-greens.gif)

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
    export const Soup = SpriteKind.create()
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

**Make a ``||variables:variable||`` to remember your Phoenix's water.**

### Make this happen

- [ ] Make a new ``||variables:variable||`` named ``||variables:phoenixWater||``.

- [ ] Set ``||variables:phoenixWater||`` to `0` in ``||loops:on start||``.

- [ ] Show ``||variables:phoenixWater||`` on Phoenix's water meter with ``||animalCare:Care Displays||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:PhoenixTrough||``.

- [ ] Inside it, change ``||variables:phoenixWater||`` by ``||variables:bucketWater||``.

- [ ] Show ``||variables:phoenixWater||`` on Phoenix's water meter with ``||animalCare:Care Displays||``.

- [ ] Set ``||variables:bucketWater||`` to `0`.

- [ ] Show ``||variables:bucketWater||`` in the bucket with ``||animalCare:Care Displays||``.

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Phoenix||`` and ``||sprites:PhoenixTrough||``.

- [ ] Inside it, change ``||variables:phoenixWater||`` by `-3`.

- [ ] Show ``||variables:phoenixWater||`` on Phoenix's water meter with ``||animalCare:Care Displays||``.

### What you should see

- [ ] Run your game.

- [ ] Fill one bucket.

- [ ] Carry it to Phoenix's trough.

The Phoenix meter should change; the other two water meters should not.

![third water: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/18-third-water.gif)

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
    export const Soup = SpriteKind.create()
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

Soup gives the ranger `20` energy.

### What to do

**Make soup give the biggest energy boost.**

### Make this happen

- [ ] Add an ``||sprites:overlap event||`` for ``||sprites:Player||`` and ``||sprites:Soup||``.

- [ ] Inside it, change ``||variables:playerEnergy||`` by `20`.

- [ ] Use ``||variables:playerEnergy||`` for the ranger's energy meter and speed with ``||animalCare:Care Displays||``.

- [ ] Destroy the soup using this event's ``||sprites:otherSprite||``.

### What you should see

- [ ] Run your game.

- [ ] Collect soup.

- [ ] Compare the three energy changes: apple `5`, sandwich `10`, and soup `20`.

Soup should give the biggest energy boost.

![complete: expected gameplay](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/19-complete.gif)

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
    export const Soup = SpriteKind.create()
}

let playerEnergy = 0

sprites.onOverlap(SpriteKind.Player, SpriteKind.Soup, function (sprite, otherSprite) {
    playerEnergy += 20
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

- [ ] Visit every creature to give it love.

- [ ] Eat a snack as your energy ticks down.

### What you should see

Each thought cloud shows its recipe from left to right. One ingredient picture means one portion and one collection trip, so repeated pictures mean repeated trips. **A** prepares food or water. **B** offers your plate in an enclosure and clears it for the next order.

- [ ] Walk up from a station to collect the food or water it prepares.

- [ ] Watch the creature names, plate spots, water meters, heart meters, and energy meter while you play.

Taking care of one creature should not quietly change another creature's values. When all three creatures have eaten, had a drink, and received love, and you have used and restored some energy, **FIRST SHIFT COMPLETE!** should appear.


![The completed first shift](https://raw.githubusercontent.com/mrbrackebusch-code/fantastic-creatures-incorporated/main/assets/demos/0a57001ffbf7/20-final-shift.gif)

## What did we learn?

Every time the game needed to remember something new, you made a ``||variables:variable||`` for it.

You ``||variables:set||`` creature choices and names by replacing what the ``||variables:variable||`` held. You ``||variables:changed||`` water, love, and energy by adding or removing an amount. You added each ingredient to ``||variables:plate||`` without removing the ingredients already there.

Look at your ``||variables:Variables||`` toolbox. How many of those ``||variables:variables||`` did not exist before the game needed them?

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
    export const Soup = SpriteKind.create()
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
    const troughX = [78, 184, 290]
    const stationX = [30, 77, 124, 174]
    const snackX = [225, 263, 301]
    const costs = [Math.abs(-7), Math.abs(-4), Math.abs(-3)]
    let ingredientKinds: number[] = []
    let snackKinds: number[] = []
    const words = ["seeds", "berries", "greens", "water", "apple", "sandwich", "soup"]
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
    let loveContact = [false, false, false]
    let drinking = [false, false, false]
    let returning = [false, false, false]
    let drank = [false, false, false]
    let meals = [0, 0, 0]
    let orders: string[][] = [["seeds"], ["berries", "seeds"], ["greens", "berries", "seeds"]]
    let servedUntil = [0, 0, 0]
    let knownIngredients = 0
    let nextDrink = [0, 0, 0]
    let unlocked = 0
    let berryHoldAt = 0
    let berryPrepared = false
    let greensTaps = 0
    let lastGreenTapAt = 0
    let pumpBeats = 0
    let lastPumpBeatAt = 0
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
            p.fillRect(2, 8, 11, 5, 14)
            p.fillRect(1, 7, 13, 2, 1)
            for (let i = 0; i < 5; i++) p.fillRect(3 + i * 2, 4 + i % 2, 2, 3, 5)
        } else if (word == "berries") {
            p.fillCircle(5, 9, 4, 2); p.fillCircle(10, 9, 4, 3); p.fillCircle(7, 5, 3, 2)
            p.drawLine(7, 3, 11, 1, 6); p.setPixel(4, 7, 1); p.setPixel(9, 7, 1)
        } else if (word == "greens") {
            p.fillCircle(4, 6, 4, 6); p.fillCircle(10, 5, 4, 7); p.fillCircle(8, 10, 4, 6)
            p.drawLine(7, 13, 4, 4, 5); p.drawLine(7, 13, 11, 3, 5)
        } else if (word == "water") {
            p.drawRect(3, 1, 9, 9, 11); p.fillRect(2, 6, 11, 8, 8)
            p.fillRect(3, 7, 9, 5, 9); p.drawLine(4, 8, 9, 8, 1)
        } else if (word == "apple") {
            p.fillCircle(5, 9, 4, 2); p.fillCircle(10, 9, 4, 2)
            p.fillRect(7, 2, 2, 4, 14); p.drawLine(9, 3, 12, 1, 6); p.fillRect(4, 6, 2, 2, 1)
        } else if (word == "sandwich") {
            p.fillRect(1, 4, 13, 3, 5); p.fillRect(2, 7, 11, 2, 6)
            p.fillRect(1, 9, 13, 2, 3); p.fillRect(1, 11, 13, 3, 5)
            p.drawLine(3, 4, 11, 4, 1)
        } else {
            p.fillRect(2, 7, 11, 5, 1); p.fillRect(4, 12, 7, 2, 11)
            p.fillRect(3, 7, 9, 2, 4); p.drawLine(5, 2, 5, 5, 1); p.drawLine(10, 1, 10, 4, 1)
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
        p.drawLine(x, y + 1, x, y + 5, 6)
        p.fillRect(x - 2, y, 5, 1, color); p.fillRect(x, y - 2, 1, 5, color)
        p.setPixel(x, y, 5)
    }

    function habitat(p: Image, slot: number) {
        let x = slot * 106 + 4
        // Grass clearings and open fences: no panel background or card border.
        oval(p, x + 6, 53, 86, 62, 7)
        oval(p, x + 14, 71, 60, 28, 6)
        fence(p, x, 55, 99)
        for (let y = 70; y < 121; y += 18) {
            p.fillRect(x, y, 3, 12, 14); p.fillRect(x, y, 2, 9, 4)
        }
        fence(p, x, 120, 17); fence(p, x + 61, 122, 38)
        // A real entrance, with stepping stones leading into the habitat.
        oval(p, x + 23, 121, 17, 7, 13); oval(p, x + 30, 132, 19, 6, 13)
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
            // Flowering grove with an asymmetrical tree canopy.
            p.fillRect(x + 78, 53, 5, 22, 14); p.drawLine(x + 80, 63, x + 70, 53, 14)
            p.fillCircle(x + 77, 48, 14, 6); p.fillCircle(x + 87, 50, 10, 6)
            p.fillCircle(x + 72, 48, 10, 7); p.fillCircle(x + 83, 43, 9, 7)
            flower(p, x + 70, 45, 1); flower(p, x + 85, 47, 3)
            flower(p, x + 10, 67, 3); flower(p, x + 18, 62, 1)
        } else {
            // A woven warm nest, rather than a third identical shelter.
            oval(p, x + 15, 77, 42, 14, 14); oval(p, x + 17, 76, 38, 10, 4)
            oval(p, x + 22, 76, 29, 6, 5)
            for (let i = 0; i < 5; i++) p.drawLine(x + 19 + i * 7, 83, x + 23 + i * 7, 87, 5)
            p.fillRect(x + 79, 55, 3, 14, 14); p.fillRect(x + 72, 53, 20, 3, 4)
            flower(p, x + 10, 57, 4); flower(p, x + 88, 67, 5)
        }
        flower(p, x + 9, 115, slot == 1 ? 3 : 5)
        flower(p, x + 91, 114, 1)
        // Trough feet and cast shadow belong to the landscape; the existing
        // overlap sprite stays centered on the actual water bowl.
        oval(p, troughX[slot] - 24, 92, 48, 10, 6)
        p.fillRect(troughX[slot] - 17, 92, 4, 9, 14)
        p.fillRect(troughX[slot] + 14, 92, 4, 9, 14)
        // The recipe rests on a little feeding mat, not a full-width footer.
        oval(p, x + 38, 111, 18 + slot * 17, 12, 4)
        oval(p, x + 39, 110, 16 + slot * 17, 9, 13)
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
        p.fillRect(0, 146, 320, 19, 13)
        for (let x = -12; x < 340; x += 38) {
            oval(p, x, 135 + x % 3, 58, 40, 13)
            p.drawLine(x + 22, 171, x + 27, 171, 4)
            p.setPixel(x + 9, 156, 4); p.setPixel(x + 25, 162, 1)
            flower(p, x + 14, 177, x % 4 == 0 ? 3 : 1)
        }
        for (let slot = 0; slot < 3; slot++) habitat(p, slot)
        fence(p, 316, 52, 4)
        for (let i = 0; i < 4; i++) {
            let x = stationX[i] - 21
            p.fillRect(x, 183, 42, 34, 14); p.fillRect(x + 2, 185, 38, 29, 4)
            p.drawLine(x + 2, 213, x + 39, 213, 5)
            p.drawTransparentImage(itemImage(words[i]), x + 14, 196)
        }
        p.fillRect(207, 184, 110, 33, 13)
        p.print("ENERGY FOOD", 232, 185, 15)
        p.print("+5", 219, 211, 15); p.print("+10", 252, 211, 15); p.print("+20", 289, 211, 15)
        p.fillRect(0, 219, 320, 21, 15)
        return p
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
        // Let the ranger leave before a replacement snack appears. Collection
        // and the energy change still belong to the learner's overlap event.
        if (nearXY(snackX[index], 202, 24)) return
        let item = sprites.create(itemImage(words[index + 4]), snackKinds[index])
        item.setPosition(snackX[index], 202); item.z = 10
    }

    function setupTrough(slot: number, kind: number) {
        let p = image.create(48, 20)
        oval(p, 0, 1, 48, 17, 14)
        p.fillRect(1, 6, 46, 9, 4)
        oval(p, 0, 0, 48, 12, 5); oval(p, 4, 2, 40, 8, 14)
        p.drawLine(4, 15, 43, 15, 14); p.drawLine(10, 14, 10, 19, 5); p.drawLine(37, 14, 37, 19, 5)
        let trough = sprites.create(p, kind)
        trough.setPosition(troughX[slot], 90); trough.z = 4
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
        if (creatures[slot] != null && value > previous) {
            // An Arcade overlap repeats every frame while the sprites touch.
            // Temporarily move the creature out of its learner-facing kind so
            // one visit produces one learner-authored change. Restore the kind
            // after the ranger has stepped away.
            loveContact[slot] = true
            creatures[slot].setKind(SpriteKind.Food)
            creatures[slot].setFlag(SpriteFlag.GhostThroughSprites, true)
            creatures[slot].vx = 0; creatures[slot].vy = 0
        }
        if (value > previous) {
            affectionAt[slot] = control.millis()
            announce(reportedNames[slot] + " loves your visit! +" + (value - previous))
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
        ranger.x += dx
        ranger.y += dy
        console.log("FCI nudge dx=" + dx + " dy=" + dy)
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
        oval(screen, x + 8, 34, 82, 23, 1)
        screen.fillRect(x + 14, 36, 70, 19, 1)
        screen.fillCircle(homeX[slot] + 17, 59, 3, 1)
        screen.fillCircle(homeX[slot] + 12, 64, 2, 1)
        if (control.millis() < servedUntil[slot]) {
            screen.print("YUM! THANKS!", x + 15, 42, 6)
        } else {
            let recipe = orders[slot]
            let start = x + 49 - Math.idiv(recipe.length * 17, 2)
            for (let i = 0; i < recipe.length; i++) screen.drawTransparentImage(itemImage(recipe[i]), start + i * 17, 38)
        }
    }

    function nextOrder(slot: number) {
        let count = Math.min(3, slot + 1 + meals[slot])
        let available = Math.max(1, knownIngredients)
        let first = Math.min(slot, available - 1)
        let recipe: string[] = []
        for (let i = 0; i < count; i++) recipe.push(words[(first - i + available) % available])
        if (count == 3) recipe[2] = recipe[0]
        orders[slot] = recipe
        console.log("FCI next-order=" + slot + " recipe=" + recipe.join(","))
    }

    function drawHud() {
        let message = statusText
        if (control.millis() > statusUntil) {
            let station = nearestStation()
            if (shiftWon) message = "FIRST SHIFT COMPLETE! Keep caring!"
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
            screen.print(chosen[slot], x + 7, 25, 15)
            drawOrder(slot, x)
            let c = creatures[slot]
            if (c != null) {
                let name = reportedNames[slot].length > 0 ? reportedNames[slot] : "- - -"
                // A high-contrast name ribbon sits beside the creature instead
                // of leaving a small word loose against the habitat art.
                screen.fillRect(x + 5, 89, 58, 11, 15)
                screen.drawRect(x + 5, 89, 58, 11, reportedNames[slot].length > 0 ? 3 : 13)
                screen.print(name, x + 34 - Math.idiv(name.length * 6, 2), 91, 1)
            }
            for (let i = 0; i < 3; i++) heart(x + 9 + i * 10, 103, reportedLove[slot] > i)
            screen.print("" + reportedLove[slot], x + 42, 103, 15)
            let width = Math.idiv(Math.max(0, Math.min(20, reportedWater[slot])) * 40, 20)
            screen.fillRect(troughX[slot] - 20, 85, width, 6, 9)
            if (width > 3) {
                let ripple = Math.idiv(control.millis(), 220) % (width - 2)
                screen.drawLine(troughX[slot] - 20 + ripple, 87, troughX[slot] - 18 + ripple, 87, 1)
            }
            screen.fillRect(troughX[slot] - 14, 102, 3, 3, 9)
            screen.setPixel(troughX[slot] - 13, 101, 9)
            screen.print("" + reportedWater[slot], troughX[slot] - 6, 100, 15)
            if (reportedWater[slot] <= 0 && c != null) {
                let warning = Math.idiv(control.millis(), 900) % 2 == 0 ? 2 : 5
                screen.drawRect(troughX[slot] - 24, 80, 48, 17, warning)
                screen.print("EMPTY", troughX[slot] - 15, 110, warning)
            }
            let splashAge = control.millis() - waterAt[slot]
            if (splashAge < 650) {
                let lift = Math.idiv(splashAge, 120)
                screen.fillRect(troughX[slot] - 7, 84 - lift, 2, 2, 9)
                screen.fillRect(troughX[slot] + 5, 82 - lift, 2, 2, 9)
            }
            let loveAge = control.millis() - affectionAt[slot]
            if (c != null && loveAge < 1200) heart(Math.round(c.x) + 12, Math.round(c.y) - 15 - Math.idiv(loveAge, 120), true)
        }
        let labels = ["SEEDS", "BERRY", "GREENS", "PUMP"]
        for (let i = 0; i < 4; i++) {
            screen.print(labels[i], stationX[i] - labels[i].length * 3, 187, 15)
            if (!stationOpen(i)) screen.fillRect(stationX[i] - 19, 197, 38, 15, 12)
        }
        let progress = [0, berryHoldAt == 0 ? 0 : Math.min(3, Math.idiv(control.millis() - berryHoldAt, 220) + 1), greensTaps, pumpBeats]
        for (let i = 1; i < 4; i++) {
            for (let j = 0; j < 3; j++) screen.fillRect(stationX[i] - 12 + j * 9, 211, 7, 3, j < progress[i] ? 9 : 14)
        }
        if (nearestStation() == 3 && lastPumpBeatAt > 0) {
            let age = control.millis() - lastPumpBeatAt
            screen.drawRect(153, 183, 42, 34, age >= 320 ? 9 : 2)
        }
        screen.print("PLATE", 5, 226, 1)
        for (let i = 0; i < 3; i++) {
            screen.drawRect(42 + i * 19, 221, 17, 17, 11)
            if (i < reportedPlate.length) screen.drawTransparentImage(itemImage(reportedPlate[i]), 43 + i * 19, 222)
        }
        if (reportedPlate.length > 3) screen.print("+" + (reportedPlate.length - 3), 101, 226, 3)
        screen.drawTransparentImage(itemImage("water"), 121, 222)
        screen.print("" + reportedBucket, 141, 226, 9)
        screen.print("ENERGY " + reportedEnergy, 181, 226, 1)
        screen.drawRect(261, 226, 53, 7, 11)
        screen.fillRect(262, 227, Math.idiv(Math.max(0, Math.min(50, reportedEnergy)) * 51, 50), 5, 7)
        if (shiftWon) {
            for (let i = 0; i < 18; i++) {
                let y = (Math.idiv(control.millis(), 40) + i * 11) % 108 + 25
                screen.fillRect((i * 43 + 17) % 318, y, 2, 3, 2 + i % 8)
            }
        }
    }

    controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
        let selected = nearestStation()
        if (!stationOpen(selected)) return
        if (selected == 0) pickup(0)
        else if (selected == 2) {
            if (control.millis() - lastGreenTapAt > 1400) greensTaps = 0
            greensTaps += 1; lastGreenTapAt = control.millis()
            if (greensTaps >= 3) { greensTaps = 0; pickup(2) }
        } else if (selected == 3) {
            let now = control.millis()
            if (lastPumpBeatAt == 0 || now - lastPumpBeatAt >= 320) pumpBeats += 1
            else { pumpBeats = 1; announce("Steady beats, not fast taps") }
            lastPumpBeatAt = now
            if (pumpBeats >= 3) { pumpBeats = 0; lastPumpBeatAt = 0; pickup(3) }
        }
    })

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
        ranger.y = Math.max(48, Math.min(210, ranger.y))
        if (!controller.A.isPressed() || nearestStation() != 1 || !stationOpen(1)) {
            berryHoldAt = 0; berryPrepared = false
        } else if (!berryPrepared) {
            if (berryHoldAt == 0) berryHoldAt = control.millis()
            else if (control.millis() - berryHoldAt >= 650) { berryPrepared = true; pickup(1) }
        }
        if (control.millis() - lastGreenTapAt > 1400) greensTaps = 0
        for (let slot = 0; slot < 3; slot++) {
            let c = creatures[slot]
            if (c == null) continue
            if (loveContact[slot]) {
                if (!nearXY(c.x, c.y, 26)) {
                    loveContact[slot] = false
                    // A greeting can occur in the same physical moment as a
                    // drink. Keep the temporary kind until the creature has
                    // also returned home, safely away from its trough.
                    if (!returning[slot]) c.setKind(creatureKinds[slot])
                    c.setFlag(SpriteFlag.GhostThroughSprites, returning[slot])
                }
            } else if (returning[slot]) {
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
                // learner still owns the actual overlap event and love change;
                // this supplied greeting only makes ordinary approaches fair.
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

    game.onUpdateInterval(3000, function () {
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
    game.onShade(function () { if (worldStarted) drawHud() })

    //% blockHidden=true
    export function startWorld() {
        if (worldStarted) return
        worldStarted = true
        // Main declares the learner-visible kinds after customts is loaded.
        // Resolve these identities on first use, never during namespace init.
        ingredientKinds = [SpriteKind.Seeds, SpriteKind.Berries, SpriteKind.Greens, SpriteKind.FullBucket]
        snackKinds = [SpriteKind.Apple, SpriteKind.Sandwich, SpriteKind.Soup]
        image.setPalette(hex`000000fff5dfe47c81f3a6bfeab46bf5dd9470a78badd49b547aa994d9dc9983bcafadb8715a70f4e6cf76564f35434e`)
        scene.setBackgroundImage(makeBackground())
        for (let direction = 0; direction < 4; direction++) for (let phase = 0; phase < 4; phase++) {
            rangerFrames.push(walkingFrame(direction, phase))
        }
        ranger = sprites.create(rangerImage(), SpriteKind.Player)
        ranger.setPosition(160, 155); ranger.z = 12; ranger.setStayInScreen(true)
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
        for (let item of value) {
            for (let i = 0; i < 3; i++) if (item == words[i]) knownIngredients = Math.max(knownIngredients, i + 1)
        }
        console.log("ANIMAL_CARE plate=" + reportedPlate.join(","))
    }

    //% block="offer $value to the creature here"
    export function servePlate(value: string[]) {
        if (ranger == null) return
        for (let slot = 0; slot < 3; slot++) {
            if (creatures[slot] != null && ranger.y < 156 && ranger.x >= slot * 106 && ranger.x < (slot + 1) * 106) {
                let recipe = orders[slot]
                let correct = value.length == recipe.length && value.length == reportedPlate.length
                for (let i = 0; i < value.length; i++) {
                    if (value[i] != recipe[i] || value[i] != reportedPlate[i]) correct = false
                }
                if (correct) {
                    meals[slot] += 1
                    servedUntil[slot] = control.millis() + 2200
                    nextOrder(slot)
                    announce(chosen[slot] + ": meal accepted!")
                    console.log("FCI meal=" + slot + " order=" + value.join(","))
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
        if (energyShown && value > reportedEnergy) ateEnergyFood = true
        if (energyShown && value < reportedEnergy) energyDecayed = true
        reportedEnergy = value; energyShown = true
        if (ranger != null) {
            let speed = Math.max(60, Math.min(130, 70 + value))
            controller.moveSprite(ranger, speed, speed)
        }
        console.log("ANIMAL_CARE energy=" + value)
    }
}
```
