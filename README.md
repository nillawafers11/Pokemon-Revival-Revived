# Pokémon Silver: Revived

Disclaimer: This is a guide on how to fix a copy of Pokémon Silver that has corroded pins. It will not cover details in depth, but rather a general overview to guide you on how to fix a copy of Pokémon for the Gameboy that has pins that are too far corroded to fix. It is intended for people with beginner/intermediate soldering skills.

I came across a copy of Pokémon Silver that was in rough shape on Facebook Marketplace for $10. It was in really rough shape based on the pictures, and seeing that I had recently taken on soldering as a hobby, I thought to myself, "I can fix it". So I met with the guy, bought it, and immediately I could tell it hadn't been cared for properly. Sticky to the touch, smelled of cigarette. I was really hoping some isopropyl alcohol would do the trick and I could call it a day. That, unfortunately, wasn't the case.

# The Inspection
Upon opening the shell by unscrewing the proprietary Nintendo screw (you need a Gamebit screwdriver, [link to iFixIt page](https://www.ifixit.com/products/gamebit-4-5mm), there are cheaper options on Amazon), I found that the pins were heavily corroded. 

Overall, the board was in bad condition and needed to be cleaned. I decided to use a toothbrush and cotton swabs with 90% isopropyl alcohol in an attempt to clean any gunk that had built onto the board. After thorough cleaning, I tried testing the cartridge inside my Gameboy Advance SP -- it didn't boot. This immediately told me one of two things; either the pins were too far corroded, or a chip on the board went bad. However, upon closer inspection, all contacts with the chips seemed to be fine. By using a multimeter and checking the traces for continuity, I was able to determine several traces leading from the pins were rusted beyond repair, and without years of experience, I wouldn't be able to fix them.

![alt text](https://github.com/nillawafers11/Pokemon-Revival-Revived/blob/main/GB/IMG_3092.jpg)

![alt text](https://github.com/nillawafers11/Pokemon-Revival-Revived/blob/main/GB/IMG_3093.jpg)

# The Plan
I was left with one option -- swap the ROM chip from Pokémon Silver board to a donor board. After some research, I came across a [Gameboy hardware database](https://gbhwdb.gekkio.fi/cartridges/mbc3.html) that lists boards that use the same mapper chip [Gameboy hardware database](https://niwanetwork.org/wiki/MBC3_(Game_Boy_mapper)). This website was crucial in helping me find a game that could give its life to save another. That game was Trade & Battle Card Hero.

While Pokémon Silver had a board model of DMG-KGDU-10 and Trade & Battle Card Hero had a board model of DMG-KDGU-01, they were functionally the same. This is because they shared the same mapper chip. All I had to do was swap the ROM chip from the Pokémon Silver board to the Trade & Battle Card Hero board.

![ROM chip circled in red](https://github.com/nillawafers11/PokemonSilverRevived/blob/main/GB/ROMchip.jpg)
