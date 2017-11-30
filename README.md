# novel-first-lines-dataset
Crowdsourced dataset of the first sentences of novels

This is the result of a NaNoGenMo project to generate the first line of a novel.

At the beginning of November, a tiny dataset produced mixed results in my first attempt to generate the first sentence of a novel http://aiweirdness.com/post/167049313837/a-neural-network-tries-writing-the-first-sentence

Highlights:
There was a man and he had seventy first sight.
It is a truth universally acknowledged, that a single man in possession of a good fortune must be in want of my life, fire of my loins.
Lowlights:
Stop! I caused the Narguuse man who was new on Alabama, the screaming constipated eggs.
I am an angry grass, the symposium square, proved fatal to the throbbing, the howling wind tire…
The really big repositories I've found (Project Gutenburg, for example) are formatted inconsistently enough that they're difficult to scrape.

So I crowdsourced a larger dataset: https://docs.google.com/forms/d/e/1FAIpQLScod8P-kcLX98u6gT0rX6-20GwkDo_glz-okVVkrhr6KgQONQ/viewform. 
It has been posted since the first week of November 2017 and as of 28 November 2017 has 11135 submissions (not all unique). 
The form is still open for submissions, and I may update this repository from time to time if the dataset size grows significantly.

Dataset stats:
11135 entries, some with authors and titles included
Some are from existing books; some are from in-progress manuscripts; some are from short stories.
Names of authors and titles are not standardized, nor are typos corrected.
Almost all entries are in English.

Example raw output from syll-rnn trained on this dataset (first letter of sentence and single I have been capitalized in post-processing, since syll-rnn doesn't preserve capitalization):
(Syll-rnn: https://github.com/learningtitans/torch-rnn/blob/valle-syllables/doc/flags.md#preprocessing )

Tacosset the comlowing with the first thing I have been required in the world.

Nothing of his brother, the path in the year of the pink world.

"ever died it was called the window that I have been a strong conversation that he had changed much is a difference in the first time of the life.

The studio was an expression to hear that he is a word and just the tour.

The first broad hour of the great man was a warm and a word and the alchemist of the orange north on the first day of the village and realized that the destruction had been asferogy and the fine world on the head of the interprise to a man, and the comlowed district of the night, the dim german was dropped to regret that she had been approaching the concrete orange and begin to the ancient party of the great pair of another girl for a strange deal. 

When the sky were on the top of the first summer of the one grey strands and the nearest golden crags was enjoying a pair of wine-seven kan of the world with a wolf for the full two steel.

The last thing of a man who was a bactrian for the west.

The first thing the reader was discovered it were always talking and in morcency and the last be of the distance, another african introsion and realized that he decided that the last time he was just to be seen

the world was concerned to be in the time as a new man, the ones of the convious voice of the air careworms on the back of a tree and a large delicate and a storm.

Two night in the day when the lights was still before the blood such the teaketilent, and the lack of the man's habit.

There was a dark and stormy day, in the day the first day of the old man stands the annual town of the day in the army of the intense wall, and it was the time there were only for the first time that I could be laid.

The truth of the oak who had been here.

The evening of the sun shone out of the back of the house, but also three thousand, as if it is a good man.

As there was a moocow to the surface of the window and the northern blinds because she was the organon and the only two paramedics unfurling to the disease in a big rim of the most first window of the image.

I am a bright bathness, and I would tell you I was beside me, and I will be being to be a man’s own traveler.

The church was the most flare of the world in the morning.

"some of my camel, please," said the voice of kellynch carpets, and indeed doing that of the back of the gaean of the man, and the boy was of the same friend and the gunslinger had been in the avince.

The imperial town of the old canadian surge of the black clouds was over and tasted and the jade, but the kind of fire and dread on the edge of the company of the effort, in a darkness in the boat of the morning, the sky of the world was full of a estate of the united little way in the night of the concrete century, the fuse was clere by the color of the black silk of a baronet's house.

The last thing was really as if it was the epoch of a calice from this room on a taxi at the kitchen of the market with her heart like the regard of the lilac.

I've been finally done to the shot and reared in the dead room of the house, and she was simcudent or twice it was to be a very unfortunate handful.

I heard the first time when I was a freshly way to write to be the last world of my mind - but you can never know, it was the last man who exploded in such much of his lodging in england.

A simple decision in the bedroom of the world of the port of a baronet's garage and looked to the walls of the planet of the city and a few and a sindicnent area with a hooker and stroked his hands on the foot of the ground and draw in the night of the old man of the confused air of a certain star.

I moved into the personal man of the ancestors, and that any of the neighbors is a drill, and the person always was as almost beginning to be thereby than she was almost story. 

The day was filled in the great land, the white contest had ever failed.

“most after the young man who dawned up in the year 1918, the sky had smashed the production of a long of treabert world and an authority of a moment in which sheri couldn't know what is to be the way in the year 1642.

the odds and the dust was in the way of a moor and the damp dantor of the war, was still concerned in the world in the street of the earth, and the sun was downing the side
