# Pokémon Silver: Revived

Disclaimer: This is a loose guide on how to fix a copy of Pokémon Silver that has corroded pins. It will not cover details in depth, but rather a general overview to guide you on how to fix a copy of Pokémon for the Gameboy that has pins that are too far corroded to fix. It is intended for people with beginner/intermediate soldering skills.

### Tools needed:
1. Gamebit screwdriver
2. Heat gun
3. Soldering iron
4. Solder
5. Flux

I came across a copy of Pokémon Silver on Facebook Marketplace for $10. It was in really rough shape based on the pictures, and seeing that I had recently taken on soldering as a hobby, I thought to myself, "I can fix it". So I met with the guy, bought it, and immediately I could tell it hadn't been cared for properly. Sticky to the touch, smelled of cigarette. I was really hoping some isopropyl alcohol would do the trick and I could call it a day. That, unfortunately, wasn't the case.

## The Inspection
Upon opening the shell by unscrewing the proprietary Nintendo screw (you need a Gamebit screwdriver, [link to iFixIt page](https://www.ifixit.com/products/gamebit-4-5mm), there are cheaper options on Amazon), I found that the pins were heavily corroded. 

Overall, the board was in bad condition and needed to be cleaned. I decided to use a toothbrush and cotton swabs with 90% isopropyl alcohol in an attempt to clean any gunk that had built onto the board. After thorough cleaning, I tried testing the cartridge inside my Gameboy Advance SP -- it didn't boot. This immediately told me one of two things; either the pins were too far corroded, or a chip on the board went bad. However, upon closer inspection, all contacts with the chips seemed to be fine. By using a multimeter and checking the traces for continuity, I was able to determine several traces leading from the pins were rusted beyond repair, and without years of experience, I wouldn't be able to fix them.

![alt text](https://github.com/nillawafers11/Pokemon-Revival-Revived/blob/main/GB/IMG_3092.jpg)

![alt text](https://github.com/nillawafers11/Pokemon-Revival-Revived/blob/main/GB/IMG_3093.jpg)

## The Plan
I was left with one option -- swap the ROM chip from Pokémon Silver board to a donor board. After some research, I came across a [Gameboy hardware database](https://gbhwdb.gekkio.fi/cartridges/mbc3.html) that lists boards that use the same mapper chip ([MBC3](https://niwanetwork.org/wiki/MBC3_(Game_Boy_mapper))). This website was crucial in helping me find a game that could give its life to save another. That game was Trade & Battle Card Hero.

While Pokémon Silver had a board model of DMG-KGDU-10 and Trade & Battle Card Hero had a board model of DMG-KDGU-01, they were functionally the same. This is because they shared the same mapper chip. All I had to do was swap the ROM chip (circled in red below) from the Pokémon Silver board to the Trade & Battle Card Hero board.
I chose Trade & Battle Card Hero because it was the cheapest option (I think I paid around $15 on eBay for it).

![ROM chip circled in red](https://github.com/nillawafers11/PokemonSilverRevived/blob/main/GB/ROMchip.jpg)

## The Removal
I will note that I recommend removing the CR2025 battery before continuing. Heat and batteries don't mix well, and this could cause it to explode. If you don't already own a soldering iron, I'd suggest getting one and looking up a tutorial on how to remove a battery from a Gameboy cartridge. It's pretty simple.

Get yourself a hot air gun, flux, and kapton tape. First, cover all components (except the ROM chip) on the board with the kapton tape. Kapton tape is a great insulator, meaning that it is good at holding heat and not transferring heat. This will protect the other components from potentially being damaged by the heat, or being desoldered off the board from the heat of the heat gun. Next, apply a liberal amount of flux on the legs of the ROM chip. Flux allows the solder to flow more uniformly over surfaces without balling up. You can now start applying heat with your heat gun.

Side note: I made the mistake of not covering ALL components with kapton tape and I accidentally desoldered a capacitor (C3 as denoted on the board). After I removed the ROM chip, the chip was covered in flux. Flux is pretty sticky when it's not hot, and I was extremely lucky that the C3 capacitor was STUCK to the ROM chip. Had I not noticed, I would've been scratching my head for days wondering why the game wasn't working.

After applying heat for about a minute onto the ROM chip, the solder was loose enough to remove the chip from the board with a pair of tweezers. I used regular metal ones but ceramic tweezers are recommended. After removing the ROM chip and battery, your board will look like this:

![ROM chip desoldered](https://github.com/nillawafers11/Pokemon-Silver-Revived/blob/main/GB/desoldedROM.jpg)

You're now going to have to do the same for the donor board (in my case, Trade & Battle Card Hero). Use the same method as stated above.

## The Transplant
After you've removed the ROM chip from both boards, you're now ready to complete the transplant. Set the old, damaged board to the side and place the donor board in front of you. This step in the process will require a lot of precision to line up the legs of the ROM chip with the pads on the donor board. My suggestion would be to cut a piece of kapton tape in half length-wise to secure the chip to the board when you have it in place. This will help in keeping it steady while you resolder the chip onto the donor board.

Apply flux to the legs again and apply heat. After a minute or so, the solder was wet and the Pokémon Silver ROM chip was now resoldered onto the donor board. In the picture below, the left board is Pokémon Silver, and the right board is the donor board with the Pokémon Silver ROM chip.

![Transplant complete](https://github.com/nillawafers11/Pokemon-Silver-Revived/blob/main/GB/IMG_3121.jpg)

I do recommend applying solder with a soldering iron to the legs of the chip to ensure that each leg is connected and secured to the board.

Then, replace the battery. I only had CR1616 batteries on hand, which will work (and what is pictured), but won't last as long. Use CR2025 batteries as denoted on the board. There is a plethora of guides online on how to replace a Gameboy battery. [Here's one from iFixit.](https://www.ifixit.com/Guide/Game+Boy+Cartridge+Battery+Replacement/27213)

Clean any residual flux thoroughly from the board with at least 90% isopropyl alcohol and you're almost done.

## The End(?)
You're going to want to test that the transplant was a success by testing it in your Gameboy. Without replacing the screw into the plastic (this just makes it easier on you in case you need to fix something), reassemble the cartridge and insert it into your Gameboy. If it boots, great! You've successfully completed the transplant and you've saved a fantastic game. You can now replace the screw and you're good to go! I went ahead and ordered a replacement label from Etsy for less than $10 because the existing label was too far gone in my opinion. Below are my results.

![It works!](https://github.com/nillawafers11/Pokemon-Silver-Revived/blob/main/GB/IMG_3125.jpg)

![The final product](https://github.com/nillawafers11/Pokemon-Silver-Revived/blob/main/GB/IMG_3139.JPG)

If it doesn't work after following the steps, proceed to the next part in this guide.

## Fixes
If you're reading this step, it means something went wrong with the transplant and your game isn't booting. There could be several issues at hand, and I'll try to list solutions to each of those issues. After attempting each solution, retest.

#### Pins are dirty
It's possible that in the transplant stage, the pins at the bottom of the board weren't cleaned thoroughly. Use a cotton swap with your isopropyl alcohol and ensure that the pins are clean.

#### The ROM chip isn't properly connected to the board
Examine the legs of the ROM chip on the board to ensure that each leg is soldered. If they aren't, reflow the solder with a soldering iron. You only need a little bit on the tip of your iron, it'll go a long way. I had to do this myself when I tested the game and it wouldn't boot.
