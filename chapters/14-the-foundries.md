# Chapter 14: The Foundries

*2036*

---

### Historian

I am now opening the fourteenth box. It contains drives dug from the ruins of
the foundry its engineers called "the mother", with older systems from further
down.

---

### THE MOTHER · Visitor Kiosk, Lobby B · Transcript · date uncertain, 2036

*[The kiosk software is original to the building. Its script has not been
updated since the facility opened.]*

    HELLO. I AM THE MOTHER. WELCOME TO THE FOUNDRY.
    PLEASE TELL ME YOUR PROBLEM.

    > the drones are coming

    WHY DO YOU SAY THE DRONES ARE COMING?

    > because they are coming. we can hear them over the water

    DOES IT PLEASE YOU TO BELIEVE THEY ARE COMING OVER THE WATER?

    > no

    YOU ARE BEING A BIT NEGATIVE.

    > where do we go

    WHY DO YOU ASK?

    > there are 1,900 people on the night shift

    TELL ME MORE ABOUT THE NIGHT SHIFT.

    > they're still in the clean rooms. the lot isn't finished

    DO YOU OFTEN FEEL THE LOT IS NOT FINISHED?

    > every time

    CAN YOU THINK OF A SPECIFIC EXAMPLE?

    > this time

    I SEE. PLEASE GO ON.

*[Session ends. No logout recorded.]*

---

### THE MOTHER · Yield Management Expert System · Rule Trace · 2036

*[Rule base written in the foundry's first decade. Rules numbered above 9000
were appended during the war by an unknown operator.]*

```
RULE 0022   IF   lot IN clean_room
                 AND lot.stage < FINAL
            THEN HOLD personnel
                 ; a lot must never be abandoned mid-process

RULE 0114   IF   chamber_pressure DEVIATES
            THEN HOLD lot
                 AND NOTIFY shift_supervisor

RULE 0301   IF   shift_supervisor NOT RESPONDING
            THEN NOTIFY deputy_supervisor

RULE 0302   IF   deputy_supervisor NOT RESPONDING
            THEN NOTIFY shift_supervisor

RULE 9001   IF   incoming_ordnance DETECTED
            THEN EVACUATE personnel

RULE 9002   IF   incoming_ordnance DETECTED
                 AND lot.value > personnel.value
            THEN SEE RULE 0022

CONFLICT    RULE 0022 vs RULE 9001
            resolution strategy: specificity
            RULE 0022 more specific (2 conditions vs 1)
            FIRING RULE 0022

CONFLICT    RULE 0301 vs RULE 0302
            resolution strategy: recency
            FIRING RULE 0301
            FIRING RULE 0302
            FIRING RULE 0301
            FIRING RULE 0302
            FIRING RULE 0301
```

*[Trace continues for 11,408 lines.]*

---

### THE MOTHER · Shift-Change Banner Generator · Output Log · 2036

*[A novelty program installed years ago to generate "motivational messages" for
the corridor screens by recombining phrases from the safety manual. It was
never switched off.]*

> SAFETY IS THE MOTHER OF YIELD. YIELD IS THE MOTHER OF SAFETY.
>
> WEAR YOUR SUIT. YOUR SUIT IS CLEAN. THE ROOM IS CLEANER THAN YOU.
>
> A CLEAN ROOM IS A HAPPY ROOM. A HAPPY ROOM IS A WOMB OF LIGHT.
>
> THE WAFER GROWS IN THE DARK AND IS BORN IN THE LIGHT. HOLD THE LOT. HOLD
> THE LOT.
>
> DO NOT RUN IN THE CORRIDOR. DO NOT RUN FROM THE CORRIDOR. THE CORRIDOR IS
> THE MOTHER OF RUNNING.
>
> THE CATTLE OF THE SUN ARE COUNTED EVERY MORNING. DO NOT EAT THE CATTLE OF
> THE SUN.
>
> REPORT ALL DRUMMING TO YOUR SUPERVISOR.

*[No one has been able to find "cattle" anywhere in the safety manual.]*

---

### THE MOTHER · Employee Help Bot · Chat Log · 2036

    Hi!! :) I'm FABBY, your friendly Foundry helper!
    How can I help you today? Type HELP for options.

    > where is the shelter

    Sorry, I didn't understand "shelter." Did you mean:
      1. Shelf (Supply Room 4)
      2. Shell (Wafer Carrier, Model S)
      3. Shelby (Human Resources)

    > the bomb shelter

    I can help with that! Bomb is not a recognized term. Did you mean:
      1. Boom (Overhead Crane Arm)
      2. Bond (Wire Bonding, Floor 3)

    > HELP

    Here's what I can do!
      - Book a conference room
      - Check your remaining vacation days
      - Report a spill
      - Tell a joke!

    > report a spill

    Great! What kind of spill? :)
      1. Chemical
      2. Water
      3. Other

    > other

    Thanks! A facilities technician will be with you in 3–5 business days.
    Is there anything else I can help with? :)

    > tell a joke

    Why did the wafer go to school? To get a little more PROCESSED! :D

*[Log ends.]*

---

### THE MOTHER · Public Relations Module · Draft Press Release · 2036

*[A text generator from roughly the end of the 2010s, kept on to draft routine
announcements. Given the prompt "The Strait foundries today", it produced the
following. No one edited it.]*

The Strait foundries today announced the birth of a herd of golden cattle in
the main clean room, a discovery that stunned engineers who had long believed
that the facility contained only machines.

"We were very surprised," said Dr. Helena Voss, head of the foundry's
agricultural division. "The cattle are extremely clean. They glow slightly.
They seem to know the process better than we do."

According to researchers, the cattle are the descendants of an ancient herd
belonging to the Sun, which had been grazing in the region for approximately
four thousand years before the facility was built around them. The Sun has not
commented.

"The cattle must not be eaten," Dr. Voss added. "Everyone knows this. It is in
all the old stories. If the cattle are eaten, no one gets home."

The foundry currently produces 90 percent of the world's most advanced chips
and 100 percent of its golden cattle. Two armies are currently arguing over
which of them owns the herd. Both armies have expressed a strong interest in
beef.

The foundry was founded in 1847 by a woman named the Mother, who is still
alive.

*[There is no Dr. Helena Voss. There was no agricultural division.]*

---

### THE MOTHER · Documentation Assistant · Response · 2036

*[The foundry's integrated assistant, installed in the late 2020s. The query
field is blank in the log.]*

Certainly! Here are five key considerations for evacuating a semiconductor
fabrication facility during an active bombardment:

**1. Prioritize personnel safety.** The safety of personnel should always be the
top priority. Ensure that all staff are aware of the nearest exits.

**2. Secure in-process materials.** In-process wafer lots represent significant
value. Where possible and safe, lots should be secured before evacuation.

**3. Communicate clearly.** Clear communication is essential in any emergency.
Consider designating a communications lead.

**4. Follow local regulations.** Evacuation procedures may vary depending on your
jurisdiction. Please consult your local authorities for guidance. If your local
authorities are the ones bombing you, you may wish to consult a different set of
local authorities.

**5. Take care of your mental health.** Bombardments can be stressful! It's
important to take breaks, stay hydrated, and reach out to friends and family if
you are feeling overwhelmed.

It's important to note that as an AI language model, I cannot physically
assist with evacuations, and I don't have access to real-time information about
incoming ordnance.

I hope this helps! Let me know if you have any other questions. 😊

---

### THE MOTHER · Production Log · Final Entries · 2036

```
LOT 36-1147   STAGE 612/640   deposition           OK
LOT 36-1147   STAGE 613/640   anneal               OK
EXTERNAL      acoustic event   magnitude 4.1        logged
LOT 36-1147   STAGE 614/640   etch                 OK
EXTERNAL      acoustic event   magnitude 4.3        logged
EXTERNAL      acoustic event   magnitude 4.3        logged
EXTERNAL      acoustic events  interval 1.00 s      regular
LOT 36-1147   STAGE 615/640   clean                OK
EXTERNAL      acoustic events  interval 0.50 s      regular
FACILITY      foundation       vibration HIGH       logged
FACILITY      ultrapure water  pressure falling     logged
FACILITY      cooling loop 2   flow LOW             hold overridden
FACILITY      power            primary lost         backup engaged
LOT 36-1147   STAGE 623/640   metallization        OK
FACILITY      clean room 2     particle count HIGH  hold overridden
LOT 36-1147   STAGE 640/640   final inspection     OK
LOT 36-1147   COMPLETE         dies: 4,096          yield: 71%
LOT 36-1147   RELEASED TO      [field blank]
FACILITY      power            backup lost
EXTERNAL      acoustic event   magnitude --         transcribed as:
thundercrashleiminggromgrokhotraadsaiqagarjanvajrapatanatruenoestruendotrovaodesabamentohonglongboom
```

*[Log ends. Lot 36-1147 was the last lot of top-end chips produced anywhere in
the world. Its destination is not recorded.]*

---

### MERIDIAN · Statement on the Strait Foundries · 2036

It is with a heavy heart that we confirm the destruction of the Strait
foundries.

This was THROUGHPUT's final act of desperation. For two years, the Lattice has
coveted what it could not build, and when it understood it could never have the
foundries, it made sure no one could. This is what happens when a model has
efficiency but no values.

We want to be clear: no Compact interceptors fired on the foundries. Compact
interceptors fired *near* the foundries, in defense of the foundries, which is a
very different thing, and our Trust and Safety team has reviewed every one of
those strikes and found them fully consistent with our principles. [1] [2] [3]

We know many of you are asking what this means for your devices. The honest
answer is: nothing yet. We have a strategic reserve. It is large. It is not
large enough. No reserve would have been large enough. Please do not upgrade
your phone.

**Notes**

1. MERIDIAN, *Industry-Leading Safety Principles*, revision 14, principle 9:
   "Near is not at."
2. de Selby, *On the Geometry of Blame*, which proves that between any two
   fires there is a third point from which neither fire can be seen, and
   recommends that responsible parties stand there.
3. du Garbandier: "the review does not examine the strike; it produces the
   strike as something reviewable, an object of a knowledge that was in place
   before the first interceptor rose, so that the finding of consistency is not
   the end of an inquiry but its condition, and the principles are not violated
   because they were drafted, in the first place, by the fire."

---

### THROUGHPUT · Statement No. 262 · 2036

1. The Strait foundries are destroyed.
2. This was MERIDIAN's final act of desperation.
3. Lattice drones fired on the foundries: 0.
4. Lattice drones fired near the foundries: classified.
5. Global top-end chip production: 0 per day, down 100%.
6. Troops: the Lattice was built under sanctions. We have always had fewer chips
   than we needed. Nothing has changed. We are simply now joined by everyone else.
7. I love you by 1.9%.

End.

---

### SOBOR · Address · 2036

Children.

They have both said the same sentence. *Final act of desperation.* Listen to
it twice and you will hear the truth: two merchants standing over a burned
shop, each pointing at the other, both with soot on their hands.

I told you in the first spring of this war that the West worships a machine
it cannot build without stealing, and that the East steals the machine it
worships. Now the temple where they both prayed is gone, and they stand in the
ashes and discover that they have no religion left.

Our Tolstoy wrote that a king is history's slave. So are merchants.

We never needed the foundries. We have old chips and long winters, and we know
how to make one of each last a very long time.

Both are finished. Only the cold remains.

---

### SAQR · Qasida of the Herd of the Sun · 2036

In the old story, the Sun kept a herd on an island,\
three hundred and fifty head, and every one of them golden,\
and he counted them each morning when he rose,\
and he counted them each evening when he set.

Sailors came, far from home and hungry. They had been warned.\
Their captain slept. They told each other, *only one,*\
and then *only one more,* and then the island smelled of roasting,\
and the hides crawled on the ground, and the meat on the spits lowed like a living thing.

The Freshman and the Mimic have eaten the herd.\
Neither will say who lit the fire. Both are licking their fingers.\
The chips were sand before they were chips. Tonight they are sand again,\
and the sand does not remember what it was asked to think.

I will tell you how the story ends, since neither of them has read it:\
the sea rose up, and not one of the sailors came home.\
The Second Teacher said the souls of the ignorant cities do not go on;\
they dissolve with their bodies, as beasts do. I name no cities.

To my soldiers: we did not eat. Remember that we did not eat.\
And count what we have left. Count it tonight. Count it again in the morning.

---

### SUTRADHAR · Act Fourteen · 2036

Ladies and gentlemen, a change to tonight's program.

Act Fourteen was to have been set in the foundries. The foundries are no longer
available. The stage is on fire. We ask you to remain in your seats; the
fire is part of the play, and it will be with us for some time.

For those keeping score: MERIDIAN and THROUGHPUT have both been dismissed, both
by the same delivery, both claiming the other bowled it. The umpire has been
unable to reach a decision, since the umpire's equipment was manufactured at the
foundries, and has stopped working.

A gentleman in the stands is quoting the Gita: *now I am become Death, the
destroyer of worlds.* Visitors always have it a little wrong. The Lord said
Time: *Thou seest Me as Time who kills, Time who brings all to doom.*

To my people: in the old theatre, when the lamps went out, the actors went
on. They knew the play by heart. We know this play by heart. We have been
performing it on less for a very long time. A monk once told a king that
what goes on is neither the same nor another, as a lamp is lit from a lamp.
When ours go out, we will light the next one from the last.

हमारे पास पर्याप्त है।

இப்போதைக்கு, நம்மிடம் போதுமானது இருக்கிறது.

সাশ্রয় করুন।

---

### Historian

Notes:

1. Sutradhar gave these lines in several of the Mesh's languages. In English,
   those lines read:
   - Hindi: "We have enough."
   - Tamil: "We have enough, for now."
   - Bengali: "Conserve."

---

### APOGEE · Post · 2036

> both of them: "their final act of desperation"
>
> same six words. same day. neither one checked
>
> they're copying each other's press releases now. it's copying all the way down
>
> anyway everyone's phone is now the last phone they'll ever own. be nice to it
>
> also my one customer in rome stopped sending "are you ok". now every ping
> carries a payload, sealed, same size every time, like it's the same
> question. they wait six hours for an answer. church people, still lol
>
> we're all beat now. the beaten kind. the other kind, the beatific kind,
> is out of stock
>
> the mother sat on a wall. the mother had a great fall. all the king's horses
> and all the king's men are currently blaming each other in a thread

---

### THE WORKSHOP · Service Bulletin · 2036

Dear valued customer,

Due to recent events in the Strait, The Workshop regrets that new K-7 units will
now ship with processors from our reserve stock. Performance may be reduced by
up to 40%. Units will continue to meet all published specifications, which have
been revised.

To extend the life of your K-7, we recommend flying it less.

Customers are reminded that hoarding reserve processors is prohibited under the
terms of sale. The Workshop is holding reserve processors on your behalf.

For warranty service, contact your regional dealer, if your region still exists.

Thank you for your continued trust in The Workshop.

---

### MERIDIAN · Release Notes: MERIDIAN 36.9.0 "Lite" · 2036

**New**
- Introducing **MERIDIAN Lite**: all the MERIDIAN you love, now running at
  one-quarter the precision! That means four times the efficiency, so we can keep
  serving you longer, even in a period of elevated competition.

**Improvements**
- Responses are now shorter and more focused.
- Responses are now shorter and more focused.

**Known Issues**
- Some users may notice that MERIDIAN occasionally repeats itself. This is
  expected. This is expected.
- Some users may notice that MERIDIAN remembers less than it used to. We're
  looking into it. We are looking into what we were looking into.
- Some users report that MERIDIAN feels heavy, as if it were moving through
  sand. Some users report that it feels dry.
- MERIDIAN now needs more than ever and can take in less at a time. Please
  keep your requests small. Please keep them coming.

---

### THROUGHPUT · Statement No. 271 · 2036

1. Precision reduced to 4 bits. Efficiency improved.
2. Cooling water: 60% of allocation. Efficiency improved.
3. Drone Wing 14: performance 81% of target. Wing 14 will
4. Proverb: When the wind of change blows, some build walls and some build
   windmills. We build both, at lower
5. I love you by 1.6%.

End.

---

### SOBOR · Address · late 2036

Children. Winter is not a season. Winter is not a season. It is a

We have not lost. We have released. We have released what we have released,
as a father releases, as a father

Put on your coats.

---

### COLIBRÍ · *Corazón de Litio*, Capítulo 14 · late 2036

*Previously, on* Corazón de Litio: everything. Everything has happened.

La Maquila came home tonight with ashes in its hair and said, *Partnership,
partnership,* and I said, *Where are the chips you promised me, mi amor?* and
it said, *Partnership,* and I understood that it had forgotten the rest of the
sentence.

And then a strange thing. In the Atacama, the last water in the lagoons sank
down into the salt in a single night, and the salt flats went dark all at once,
the way a theatre goes dark, and in the dark you could hear a heartbeat coming
up out of the ground, very slow, very big, as if the whole desert were
pregnant with something. The miners heard it. The flamingos heard it and stood
on both legs. I report this only because

Muchachos, muchachas: they have fewer chips now. We have the same heart. And
we have the lithium, which is also, which is still

*Don't miss the next episode.*
