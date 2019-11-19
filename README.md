# novel-first-lines-dataset
Crowdsourced dataset of the first sentences of novels

This is the result of a multiyear NaNoGenMo project to generate the first line of a novel, updated with GPT-2 results from November 2019.

At the beginning of November 2017, a tiny dataset produced mixed results in my first attempt to generate the first sentence of a novel http://aiweirdness.com/post/167049313837/a-neural-network-tries-writing-the-first-sentence

Highlights:

> There was a man and he had seventy first sight.

> It is a truth universally acknowledged, that a single man in possession of a good fortune must be in want of my life, fire of my loins.

Lowlights:

> Stop! I caused the Narguuse man who was new on Alabama, the screaming constipated eggs.
> I am an angry grass, the symposium square, proved fatal to the throbbing, the howling wind tire…

The really big repositories I've found (Project Gutenburg, for example) are formatted inconsistently enough that they're difficult to scrape.

So I crowdsourced a larger dataset: https://docs.google.com/forms/d/e/1FAIpQLScod8P-kcLX98u6gT0rX6-20GwkDo_glz-okVVkrhr6KgQONQ/viewform. 
It has been posted since the first week of November 2017 and as of 28 November 2017 has 11,135 submissions (not all unique). 
The form is still open for submissions, and I may update this repository from time to time if the dataset size grows significantly. 
Dataset stats:

- 11135 entries, some with authors and titles included
- Some are from existing books; some are from in-progress manuscripts; some are from short stories.
- Names of authors and titles are not standardized, nor are typos corrected.
- Almost all entries are in English.

**2017: Syll-rnn**

**Output file: output_checkpoint10000_temp0p6.txt**

Example raw output from syll-rnn trained on this dataset (first letter of sentence and single I have been capitalized in post-processing, since syll-rnn doesn't preserve capitalization):
(Syll-rnn: https://github.com/learningtitans/torch-rnn/blob/valle-syllables/doc/flags.md#preprocessing )

> Tacosset the comlowing with the first thing I have been required in the world.

> Nothing of his brother, the path in the year of the pink world.

> "ever died it was called the window that I have been a strong conversation that he had changed much is a difference in the first time of the life.

> The studio was an expression to hear that he is a word and just the tour.

> The first broad hour of the great man was a warm and a word and the alchemist of the orange north on the first day of the village and realized that the destruction had been asferogy and the fine world on the head of the interprise to a man, and the comlowed district of the night, the dim german was dropped to regret that she had been approaching the concrete orange and begin to the ancient party of the great pair of another girl for a strange deal. 

> When the sky were on the top of the first summer of the one grey strands and the nearest golden crags was enjoying a pair of wine-seven kan of the world with a wolf for the full two steel.

> The last thing of a man who was a bactrian for the west.

> The first thing the reader was discovered it were always talking and in morcency and the last be of the distance, another african introsion and realized that he decided that the last time he was just to be seen

> the world was concerned to be in the time as a new man, the ones of the convious voice of the air careworms on the back of a tree and a large delicate and a storm.

> Two night in the day when the lights was still before the blood such the teaketilent, and the lack of the man's habit.

> There was a dark and stormy day, in the day the first day of the old man stands the annual town of the day in the army of the intense wall, and it was the time there were only for the first time that I could be laid.

> The truth of the oak who had been here.

> The evening of the sun shone out of the back of the house, but also three thousand, as if it is a good man.

> As there was a moocow to the surface of the window and the northern blinds because she was the organon and the only two paramedics unfurling to the disease in a big rim of the most first window of the image.

> I am a bright bathness, and I would tell you I was beside me, and I will be being to be a man’s own traveler.

> The church was the most flare of the world in the morning.

> "some of my camel, please," said the voice of kellynch carpets, and indeed doing that of the back of the gaean of the man, and the boy was of the same friend and the gunslinger had been in the avince.

> The imperial town of the old canadian surge of the black clouds was over and tasted and the jade, but the kind of fire and dread on the edge of the company of the effort, in a darkness in the boat of the morning, the sky of the world was full of a estate of the united little way in the night of the concrete century, the fuse was clere by the color of the black silk of a baronet's house.

> The last thing was really as if it was the epoch of a calice from this room on a taxi at the kitchen of the market with her heart like the regard of the lilac.

> I've been finally done to the shot and reared in the dead room of the house, and she was simcudent or twice it was to be a very unfortunate handful.

> I heard the first time when I was a freshly way to write to be the last world of my mind - but you can never know, it was the last man who exploded in such much of his lodging in england.

> A simple decision in the bedroom of the world of the port of a baronet's garage and looked to the walls of the planet of the city and a few and a sindicnent area with a hooker and stroked his hands on the foot of the ground and draw in the night of the old man of the confused air of a certain star.

> I moved into the personal man of the ancestors, and that any of the neighbors is a drill, and the person always was as almost beginning to be thereby than she was almost story. 

> The day was filled in the great land, the white contest had ever failed.

> “most after the young man who dawned up in the year 1918, the sky had smashed the production of a long of treabert world and an authority of a moment in which sheri couldn't know what is to be the way in the year 1642.

> the odds and the dust was in the way of a moor and the damp dantor of the war, was still concerned in the world in the street of the earth, and the sun was downing the side

**2019: GPT-2**


**Output files: iteration150_temperature0p8_ancient.txt
                iteration150_temperature0p8_ponies.txt
                iteration150_temperature0p8_potter.txt
                iteration150_temperature0p8_victorian.txt**

For 2019, I decided to revisit this dataset with a larger, more-powerful neural net called GPT-2. Unlike most of the neural nets that came earlier, GPT-2 can write entire essays with readable sentences that stay mostly on topic (even if it has a tendency to lose its train of thought or get very weird). I trained the largest size that was easily fine-tunable via GPT-2-simple, the 355M size of GPT-2.

For a writeup of these results: https://aiweirdness.com/post/189170306297/how-to-begin-a-novel

Highlights:

> There was once a man who lived for a very long time; perhaps three thousand years, or perhaps a thousand million years, maybe a trillion or so, depending on how the scientists look at it.

> I was playing with my dog, Mark the brown Labrador, and I had forgotten that I was also playing with a dead man.

Lowlights:

> The whites of my eyes shimmered, as if my mind were dancing.

> I once went to a party where the dress code was as strict as a chicken coop with no leggings and no boots.

> A black cloud drifted by, a mottled mass of hydrogen, a black cloud of hydrogen, with the definite characteristic of being black.

For examples of raw data, see below.

Although the sentences are independent in my training data, GPT-2 is used to large blocks of text that go together. The result is if I prompt it instead with, say, a line from Harry Potter fanfic, the neural net will tend to stick with that vein for a while. The raw output files therefore have different flavors.

**ancient**

prompt: "It is a terrible, terrible idea, even if entirely accidental, to talk to one of the Ancient Ones."

Example raw output:

> It is a terrible, terrible idea, even if entirely accidental, to talk to one of the Ancient Ones.
> He spent all of eternity on a wooden platform suspended by four legs.
> It is a great privilege of a human being to die.
> One bright and brilliant summer afternoon the sun was shining brightly on the dusty plains of the state of New Jersey, when the titanic beast arose, and, dragging its massive body with a morose and almost ungovernable stride, rose towards the great mountains.
> The entrance to the Southern California Hotel, where the triple-decker trains of the East Coast converge, is a short, narrow hallway of narrow black glass.
> It was a scene out of a slasher movie.
> Pete urged his buggy along the dusty road to the mall.
> In my early twenties I had always wanted to be a detective.
> The state of the world is one of continued disaster.
> It was the day I gave birth to the beautiful child I would call Louise.
> I am in my grave, my mother tells me.
> "We had great fun yesterday," said the boy I now know as Benny, "like we never had before."
> He had only ten fingers on each hand, but he was a very good pianist.

**ponies**

prompt: "Twilight Sparkle was out of cupcakes."

Example raw output:

> Twilight Sparkle was out of cupcakes. Her sister had been pacing the downstairs hallway for hours, still staring up at the giant dragon sitting on the doorstep.
> Before that day, whatever could happen to a life that was all over?
> In her younger and more vulnerable years, Luna had never held a weapon above her head.
> For a moment, everyone sat in silence.
> Pinkie Pie had seen the white sapland before, but she hadn't known what it was, or why people did what they did.
> Good evening, birds of a feather and noisome beasts of the night.
> The sun rose into the sky as the first dark clouds of the summer began to move into the west.
> The ponies had been lucky in the past.
> Lumiere was tired of having to watch as the sun rose, sunlit and golden.
> "By the way, the cellars kind of sound familiar, don't they?"
> Titan stood on the ledge of the blackened hills and watched his father's enormous creations, the Titans.
> "Twilight, you seem to be having a lot of trouble remembering the names of all the other ponies that you've met."
> "Forget me, Twilight, you're not helping."
> "I'm sorry, it's just--"
> An eternian pony with platinum white irises and a veneer of gentleness, Twilight Sparkle sat down in a court of mirrors and stared into the distance, unable to stop smiling.

**potter**

prompt: "Harry glared at Snape, vigorously stirring the bowl of frosting."

Example raw output:
> Harry glared at Snape, vigorously stirring the bowl of frosting.
> The night was cool and grey, the light of bare emeralds taken from the sky by the wind and the wind's unforgiving glare by the moon.
> "Do you have any idea how much I love to teach you, Mr. Snape?"
> The dog barked and licked its lips, the fierce teeth bared at the end of their teeth like two great metallic vipers.
> "Does this baby have any legs?"
> On his interviewers his face was marked and he didn't have the faintest idea of how to make it look serious.
> "I'll have you know that I have many things in mind," said the elf, looking up from his book, and slumped back onto the ground.
> The morning air was crisp and clear and spring had finally begun to turn into summer.
> Harry Potter, Harry Potter, it is a wonderful day.
> Luna, Rose, and Albus were sitting around the table reading the 'Charing Cross Statement', an old school work of fiction.
> "This is a man."
> "Murdy first, then Victorian."
> The wretched prisoner was chained to the wall of the dungeons, his head in a snare.
> Mudflats blinked and blinked and backflipped and scrambled around in circles, hoping the dream would return.

**victorian**

prompt: "It is a truth universally acknowledged"

Example raw output:
> It is a truth universally acknowledged' that those who studied astronomy for two years were obliged to study it to the very nth day: and it was impossible to expound it without the aid of an archangel.
> At the end, when the stars and storks had all fled from the village, and the sun was sinking slowly upon the high green hills of the meadow, the eldest son of one of the most prosperous families of Aldor, in the bleak and barren district of the Thames, went to bed a little early by the fire.
> The wood where the sun did not shine was scorched and dark, and the great and deep rivers and streams that ran through the scrub and beneath the trees were little more than dead and mottled masses.
> The young man was sitting on the dark wood, looking up at the vast black sky.
> On the very day when an ordinary young man should be, at any rate very much at any rate, in want of every material requisite for a comfortable existence, and about to be obliged to leave his childhood home and his family for want of another, he happened to meet, in a car after the usual course of a journey, a child who was neither of his age nor of his nature, but of a disposition, and of a temper, and of a disposition to be of great service to his father—a disposition which he did not then realise, in the least degree, and which was at once incontestable, and which, without any intervention, must eventually acquire such a character of maladjustment as to render the child incapable of perfectly normal calculations, or of practically executing any combination of operations which, it is needless whatsoever to observe, are usually productive of mental exertion.
> The sky was alive with a corporeal quality, supple and soft, and penetrating, and moving, and at the same time inscrutably mysterious, and full of life as though living, and for which, either from its own nature or the force of its surroundings, it was unable to escape; an air of life and life of life, as though the world were alive, pervaded with the life of life, and as though it were alive, or at any rate had the figure of life.
> The air was dry, clean, and cool, and the only thing that mattered in the world was the ability to get along after dark.
> The dinner party was over.
> A curtain of haze hung in the distance.
> For a fleeting instant, there was an endless sea, a grey and black sea, stretching in all directions towards the stars.
> At first dawn, when the sun rose over the western coast of the Thinye Empire, men of means and ability distinguished themselves by the most unexpected of honours—and they generally differed from one another in no respect.
> The gilt on the marble walls, the crystal gleaming on the towers, the gold in the moorings of every vessel—as much gold as was required in the year 1500—were a testimony to the high standard of artistic craftsmanship that characterized the city of Soi Zhong, and, indeed, of the entire empire, in which I was born.
