# TakeMeter

> ### 👋 Start here
>
> **New to this repo? Read [RUNNING.md](RUNNING.md) first** — setup, the
> notebook, the baseline, and what to do when something breaks.
>
> Once `python test.py` passes:
>
> ```bash
> head -5 data/practice_labels.csv     # the shape your labels.csv needs
> ```
>
> Then open `takemeter.ipynb` **in this folder** — in VS Code, or with
> `jupyter notebook` if you prefer. Pick the kernel: the `.venv` inside this
> project. Run section 1, which reports the hardware you'll be training on.
> Everything else waits until you have data.
>
> Nothing to upload, nothing to connect, no accounts and no keys. The notebook
> runs on your machine and writes next to your code.
>
> **The rest of this file is your submission.** Fill it in as you go.

---

<!-- ─────────────────────────────────────────────────────────────────────────
     HOW TO USE THIS FILE

     Unit 5 asks for the first five sections. Unit 6 adds the five below them.

     Everything is pasted as TEXT. No screenshots, no images.

     ⚠️ The confusion matrix especially. The notebook prints one as a markdown
     table, ready to copy. A screenshot of a matrix earns nothing. Paste the
     table.
     ───────────────────────────────────────────────────────────────────────── -->

<!-- ═══════════════════════ UNIT 5 — THE BUILD ═══════════════════════ -->

## What This Does

<!-- Your community, and what your classifier sorts posts into. Three or four
     sentences. -->

There is a 

---

## Label Taxonomy


### `Reasoned Opinion`

**Definition:** Gives judgement (whether good or bad), but includes an explanation of why based on lyrics, instrumental, vibe, etc.

**Example 1:**
> 
BLUE BLOOD: Strong opener. Interesting instrumental. It would work very well as an opener for their tours similar to aespa’s AENERGY.

I AM: Pop heaven for a Pop Brat like me. The notes are a bit too high at some points, but it’s a very catchy tune. I love the second verse. Gaeul’s rap is a great break from the high-pitched nature of the song. Liz, Liz, Liz! She sounds lovely.

KITSCH: I liked it when I first heard it and still do but listening to this album and comparing it to their previous tracks, it’s pretty basic and doesn’t stick out in any particular way. The verses are good, but reminiscent of early to mid-2010s pop with a tiny hint of nostalgia. The chorus, while an earworm, is repetitive and kind of throws the song off in a way. I’m not sure if it’s in an entirely bad way, just that it feels odd. The rap bridge was … interesting. I like the way the pre-chorus sounds after the bridge, though.

LIPS: It’s a mood, it’s a vibe, it’s paradise. It’s a cute little summer beach tune (we southern hemisphere citizens are heading into winter soon but okay). Nothing much to say. It’s just cute!

HEROINE: Vocals are great. That whoo na-na-na-na section took me by surprise but I love it. The track doesn’t stick out in a particularly good or bad way.

MINE: This is the track that I claimed from the highlight melody and I’m happy to report that it has not disappointed me. I love the melody and the “bounciness” of the song. It reminds me of a very specific sound from the early to mid-2010s in a good way. I really like the tempo, the instrumental, and the way it’s sung. The section that they used for the snippet from the highlight medley is very catchy. I really like this song and it’s going on my daily playlist.

HYPNOSIS: It makes me feel like an under-the-radar badass. “Cool” is the only word that I can use to describe this song. I like the instrumental and whatever’s happening in the background. It’s what SHOOT and Gas Me Up are to ITZY. It also sounds like it could have been a track on aespa's Savage album. Maybe even the Girls album (Illusion's sister).

NOT YOUR GIRL: I’m first and foremost a Pop Brat and this song is everything, everything, everything! It’s a song that very much lifts your spirit and puts you in a good mood. It’s got a catchy melody and good vibes. Love it! It’s too bright to put in my daily playlist, but there’s a place reserved for it somewhere on one of my main playlists.

NEXT PAGE: It’s nice. It’s got a filler-y quality about it, though. It doesn’t stick out as particularly good or bad. They sound great, though.

CHERISH: Groovy instrumental! Their vocals are lovely on the track. But my feelings about it are the same as Next Page.

SHINE WITH ME: It’s fine. Good, even. The instrumental is very pretty. It’s a bit too ballad-y for my taste, though, especially since my mood is all out of sorts (PMS) and I’m craving some upbeat music.

In conclusion, it’s a solid album. Some tracks stick out more than others, but that’s to be expected with a full album. The songs that didn’t hook me have the potential to grow on me. The songs that hooked me are among my favourite releases from the year so far. It's missing a strong track like My Satisfaction (which is still one of their best songs) but it's diverse enough to lay the foundation of what might become their signature sound.

**Example 2:**
My first thoughts (editing/adding when I'm done listening):

Blue Blood : Nice, a good opener, but I feel like the song doesn't really go anywhere? I'd say a solid 7/10 for me

I AM: it's a great title. 9/10 because some passages sound a bit empty to me but overall really good.

Kitsch: I instantely liked this song when it came out and still think it holds up great. I don't think the place in the tracklist makes too much sense, having it directly after I AM is a bit overwhelming. But the song is still a 9/10.

Lips: Ohhh I really really like this! 9/10, maybe even 10/10 in a few days, it's definitely added to my playlist.

Heroine: It's nice. I like their voices, they sound really good in this. Also the brige buildup to the last chorus is >>>. A good b-side, not extraordinary but solid. I think the rating may improve with more listens. 7.5/10

Mine: The first neutral song for me. It's not bad, I wouldn't play it again though. 5/10

Hypnosis: that intro, I almost thought my headphones broke. Changes up the sound, I like that! The rythm is definitely hypnotizing. The song itself isn't it for me, but I applaud them for doing something different so bonus points for that 6/10.

NOT YOUR GIRL: Ohh it's cute. It's fun. An instant mood boster. It reminds me of the songs that are played during a makeover montage in a teen movie. 9/10, will add this to my getting ready playlist for sure.

Next Page: I'm really not sure what to think of this song. I do like it, but also something is missing I just don't really know what? Unfortunately only a 6/10 so far.

Cherish: I like the pre-chorus. The chorus itself falls a bit flat for me. It's a nice song and a good b-side but a bit too repetitive for my taste. The girls sound good though. It's also mixing up style and tempo quite a lot which is nice. 7/10.

Shine With Me: A classic closing ballad. The lyrics are really good and feel very personal - this is a song for DIVE right? 8.5/10.

Overall: The album has some solid bangers and good b-sides. Some songs fall a bit flat for me but with 11 songs in an album that's completely okay and to be expected, and maybe those songs are the favorite songs of other people (I'm seeing a lot of people being into Hyponsis!) . Overall they offer a good variety of styles, sounds and themes all while maintaining a certain IVE-style. It's a great album, one I'll definitely come back to listen often (and maybe even order a physical copy).

### `Unreasoned Opinion`

**Definition:** A claim about the album or a song but has no reason of why they think that way. 

**Example 1:**
Not a single skip in my opinion. What a perfect first album.


**Example 2:**
Not your girl giving me the song of summer vibes.


### `Emotional Reaction`

**Definition:** A comment that mainly expresses a feeling (excitement, love, frustration, humor) rather than explaining a judgment. It may hint at an opinion, but gives no reasons for it.

**Example 1:**
Rei ran out of rap. That’s why she said she needed to do better hahah

Kidding aside…it makes you want to repeat it dontcha think??

**Example 2:**
girl why is hypnosis so short!!!!! i neeed more sound like this from ive!!!!!

### The hardest boundary

**Which two labels:** Emotional Reaction and Unreasoned opinion

**The decision rule I used every time:**
If the post states a claim (good or bad) about a song or album ("this song is really good!"), it can be an unreasoned opinion. If it only expresses a feeling (excitement, love, frustration, humor) without claiming anything about the song's quality, it's an emotional reaction ("this gives me goosebumps!!"). When a comment does both, I labeled it by the main point: a verdict on quality made it an unreasoned opinion, and a feeling or joke made it an emotional reaction.


---

## The Dataset

<!-- Where you collected from, how you labelled, your counts, and three hard
     cases. -->

**Where the posts came from:** Reddit r/kpop -> a post called "IVE - I've IVE (The 1st Album)"

**How I labelled them:** I did 23 cold first then pre-labeled with AI then corrected.

**Counts per label:**

| Label | Count | Share |
|---|---|---|
| Reasoned Opinion | 101 | 49.5% |
| Unreasoned Opinion | 83 | 40.7% |
| Emotional Reaction | 20 | 9.8% |
| **Total** | 204 | 100% |

**Three hard cases**

**1.**
> *The post:* Cherish got me doing body rolls why does it go so hard
>
> *Could have been:* Unreasoned Opinion
>
> *I chose, because:* Emotional reaction, because although it could be an opinion, it leans more towards emotional reaction because of the exaggerated "body rolls".

**2.**
> *The post:* I am honestly blown away by this album, and pretty emotional ngl lol. My favorites so far: Blue Blood, Lips, Heroine, Hypnosis (ARE THEY KIDDING MEEE???), and Next Page.
>
> *Could have been:* Unreasoned Opinion
>
> *I chose, because:* Emotional reaction, because the "ARE THEY KIDDING MEEE???" and the "pretty emotional" shows the main point is the emotions they felt and their reactions rather claiming a song is really good (does lay out favorites but no claims about them).

**3.**
> *The post:* Just wanted to drop by and say Cherish’s chord progression gave me a nice little brain itch and I don’t see enough appreciation for it.”
>
> *Could have been:* Unreasoned Opinion
>
> *I chose, because:* Reasoned opinion, because the main claim is that they enjoy the song "Cherish" which is shown by the "I don't see enough appreciation for it" while the reason is "Cherish's chord progression". 

---

## The Training Run

**Base model:** `distilbert-base-uncased` (fine-tuned for sequence classification)

**Settings:** 2 epochs, learning rate `1e-4`, batch size 16, seed 42 (maximum
sequence length: 128 tokens)

**Anything I changed from the defaults, and why:**Changed 2e-5 learning rate to 1e-4 learning rate and 3 epochs to 2 epochs. I changed to 1e-4 so that the model wouldn't learn too slow, requiring more epochs. By doing that, I also had to lower the epochs since I noticed it reached a min of loss at 2 epochs.

**Split sizes:**
                    train  val  test
label                               
Reasoned Opinion       71   15    15
Unreasoned Opinion     57   13    13
Emotional Reaction     14    3     3

Note: Emotional Reaction only has 3 examples for both val and test set.



---

## How I Used AI

**Moment 1**

- *What I asked for:* To pre-label the text.
- *What came back:* a new .csv file with labels for each text and a note (that I edited with "checked" after checking).
- *What I changed:* A few of the labels were not what I thought they should be and I changed them.

**Moment 2**

- *What I asked for:* Give examples of numbers to use for criteria.
- *What came back:* Gave me examples (like range of numbers or units) for each criteria.
- *What I changed:* I changed the range or number to fit what I wanted. I just needed the unit.

**Pre-labelling disclosure:** I pre-labeled but checked the labels on my own.

<!-- ═══════════════════════ UNIT 6 — THE TEST ═══════════════════════

     Don't fill these in during unit 5.
     ═══════════════════════════════════════════════════════════════════ -->

---

## Baseline vs. Trained

<!-- Both models on the same posts. `python baseline.py --trained results.json`
     prints this table for you. -->

| Measure | Baseline | Trained | Difference |
|---|---|---|---|
| Overall accuracy |  |  |  |
| Macro F1 |  |  |  |
| F1 — `label_one` |  |  |  |
| F1 — `label_two` |  |  |  |

**What I predicted before I looked:**
<!-- Milestone 1 asks you to write this BEFORE seeing the trained numbers. A
     prediction made afterwards isn't one. -->

**What the gap actually means:**
<!-- If the baseline matched your trained model, your fine-tuning added
     nothing — and that is a real finding, not a failure. Say it plainly. -->



---

## Run Log — Before

<!-- Five criteria across three seeds. The notebook's section 6 prints the
     spread table; the Target and Verdict columns are yours. -->

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

### Confusion matrix

<!-- ⚠️ TYPED AS A MARKDOWN TABLE. The notebook prints one ready to paste.
     An image of a matrix earns nothing. -->

| true \ predicted |  |  |  |
|---|---|---|---|
| **** |  |  |  |
| **** |  |  |  |
| **** |  |  |  |

**My biggest off-diagonal number, and what it means:**
<!-- Not "the model made mistakes" — WHICH boundary it didn't learn, and which
     direction. "7 real analysis posts were called hot_take and only 3 went the
     other way" is a direction, not just an error rate. -->



---

## Verdicts and Diagnoses

<!-- MET or MISSED against LAST UNIT's target. The target has to hold across
     all three seeds, not turn up sometimes. -->

| # | Criterion | Target | Verdict | How I decided |
|---|---|---|---|---|
| 1 |  |  |  |  |
| 2 |  |  |  |  |
| 3 |  |  |  |  |
| 4 |  |  |  |  |
| 5 |  |  |  |  |

**Diagnoses**

<!-- For each miss: the cause, and how you know. The four common causes are:
     too few examples for a label, a boundary you applied inconsistently, a
     genuinely hard label pair, and a task the model can't reach from this
     much data.

     ⚠️ Use your agreement report as evidence. It is the only instrument you
     have that can tell a LABELLING problem from a MODEL problem, and this
     section is graded on whether you used it that way. -->



---

## Agreement Report

<!-- Your rate against the staff set, and every disagreement adjudicated.

     Remember you labelled these 30 under the STAFF taxonomy in
     data/staff_taxonomy.md, not your own — so every argument below is made
     from those definitions and those decision rules. -->

**Agreement rate:** ___ / 30 = ___%

<!-- Nobody grades this number. A 60% who argues every disagreement from the
     stated rules beats a 95% who wrote "staff was right" nine times. Several
     of the 30 were chosen because they're genuinely ambiguous — you should be
     winning some of these. -->

**Disagreements**

<!-- Three lines each: the post, both labels, and who you think is right and
     why — grounded in the staff definitions you were both applying.

     Then sort each into one of three piles:
       (a) the rule covered it and I applied it loosely → a consistency problem
       (b) the rule genuinely doesn't say               → a gap in the definitions
       (c) the rule is ambiguous here and my reading is defensible → argue it.
           This is a legitimate win.

     Pile (a) is the one that matters most for your diagnosis: if you applied a
     written rule two different ways on 30 posts, that is direct evidence about
     what you did across your own 200. -->

**1.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**2.**
> *The post:*
>
> *Staff said / I said:*
>
> *My call, and why:*
>
> *Which pile:*

**What the pattern in my disagreements tells me:**



---

## The Improvement

**What I changed:**

**Which diagnosis pointed at it:**

### Run Log — After

| Criterion | Target | Seed 42 | Seed 7 | Seed 2024 | Verdict |
|---|---|---|---|---|---|
| 1.  |  |  |  |  |  |
| 2.  |  |  |  |  |  |
| 3.  |  |  |  |  |  |
| 4.  |  |  |  |  |  |
| 5.  |  |  |  |  |  |

**Did it help, and how do I know:**

<!-- If it didn't, say so. Relabelling that didn't help is a genuinely
     interesting result and earns full credit. -->



---

## What's Still Broken

<!-- For each criterion still missed: what you'd do, and why you stopped. -->



**The gap between what I meant my labels to capture and what the model
learned:**
<!-- Two sentences. Your confusion matrix is the evidence. -->



<!-- ═════════════════════════════════════════════════════════════════════

     SUBMISSION CHECKLIST — unit 5

       [ ] criteria.md has five numbered criteria, each naming a NUMBER
       [ ] Each has a reason underneath tied to your data or taxonomy
       [ ] labels.csv: at least 150 rows, text/label/note, ONE file not split
       [ ] No label above 70%
       [ ] All five unit 5 sections have real content
       [ ] Label Taxonomy includes the decision rule for your hardest boundary
       [ ] The Dataset includes three hard cases
       [ ] results.json and test_split.csv committed (the notebook does this)
       [ ] At least four new commits
       [ ] Repository URL submitted — WRITE IT DOWN

     SUBMISSION CHECKLIST — unit 6

       [ ] Baseline vs. Trained table, with your prediction written beforehand
       [ ] Run Log — Before, five criteria across three seeds
       [ ] Confusion matrix TYPED AS A MARKDOWN TABLE
       [ ] A verdict on every criterion
       [ ] A diagnosis for every miss, using the agreement report as evidence
       [ ] Agreement Report with every disagreement adjudicated
       [ ] One improvement, with Run Log — After
       [ ] What's Still Broken
       [ ] results_three_seeds_before.json, results_three_seeds_after.json,
           baseline_results.json and
           agreement_results.json committed
       [ ] At least four new commits
       [ ] The SAME repository URL as last unit

     Do not delete and recreate this repository.
     ═════════════════════════════════════════════════════════════════════ -->

---

📖 **How to run this project: [RUNNING.md](RUNNING.md)**
