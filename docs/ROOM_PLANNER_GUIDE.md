# GSonic Evo 32 — the Room Planner, a user guide

*For GSonic Evo 32 2.1.0 and later. The Room Planner is an experimental tool: a model of your room, not a measurement.
Read its map as places worth trying; the calibration's own measurement decides.*

---

## 1. What it is, and what it is not

The Room Planner is a playground for subwoofer placement. You draw your room, put the seats and the speakers in
it, and the planner shows where a subwoofer would smooth the bass best across your seats — before you move anything.
It opens from the **Planner** entry in the sidebar, in its own window.

It is independent of the calibration. Nothing you do in the planner changes a run, a filter or the receiver. You can
open it, play with it and close it; your calibration is exactly what it was.

It ranks positions with a simplified picture of your room: flat rigid walls, one damping value for the whole room, no
furniture, no open doors. Real rooms differ from that picture by a few dB, and by more above about 100 Hz. So the
planner's answer is a shortlist of places worth trying, not a verdict. The way to use it is always the same: move the
subwoofer to a spot the planner likes, measure, run the calibration, and keep the placement that measures best. If a
move makes the calibration worse, move back.

**What it can tell you**

- Where the bass is smoothest across your seats — for one subwoofer, or for two to four placed together — with each
  subwoofer's delay, level and polarity set as a calibration would set them.
- How the room's modes fall on your seats: a pressure map at any frequency, and the list of modes below 200 Hz.
- Whether the model fits *your* room: opened from a measured session, it compares the subwoofer sweep your calibration
  recorded with its own prediction and says in plain words how far the map can be trusted.

**What it cannot tell you**

- Anything the calibration measures: the real response, the real delays, the real crossover. The planner is a sketch;
  the measurement is the fact.
- Anything above the bass. The model stops being useful above roughly 100 Hz.
- What furniture, openings and the walls' construction do. A real room is leakier and more damped than the model, and
  the measurement check shows by how much.

## 2. How it fits into your measurements

The planner does not make a measurement better or replace one. It uses your measurement twice, and it tries to save
you rounds of moving and re-measuring:

1. **Measure as usual** with GSonic Immersive and run the calibration in Evo 32.
2. **Open the planner from that session** (the sidebar's Planner entry; leave "start from this session's speakers and
   crossover" ticked). The planner places your front speakers in the directions the measurement found them, takes the
   crossover from the run, and knows whether your fronts are sealed or ported and where they roll off.
3. **Draw your room** and give it the distances only you can measure: the seat to the left front speaker, left speaker
   to right speaker, the fronts to the front wall, the tweeter height, your ear height.
4. **Check the model against your measurement.** Put the subwoofer on the plan where it stood when you measured and
   press *Check the model*. The planner compares the subwoofer sweep your calibration recorded with its own prediction
   at your seats and tells you whether the map can be trusted in your room.
5. **Find the best spots** for one subwoofer, or the best arrangement of all of them.
6. **Move, measure again, run the calibration again**, and compare. The measurement decides. A move that measures
   worse is a move to undo.

The planner's value is in step 5: instead of trying every corner by hand, you try the two or three places the model
ranks highest, and you know from step 4 how much weight its ranking deserves in your particular room.

## 3. Step 1 — your room

**Shape.** Start with a rectangle (width, length, ceiling height, in metres or feet). If your room is not a rectangle,
switch to *any outline*: start from the L-shape, trapezoid or bay preset, then drag the square corners on the plan,
click a wall's round middle handle to add a corner there, and double-click a corner to remove it. Draw the room with
the front wall — the speakers' wall — at the top of the plan. Width runs left to right, length front to back.

Partial-height alcoves and window bays below the ceiling cannot be drawn; the planner takes a floor outline. Leave them
out.

**Getting the outline and the dimensions.** A tape measure is all a rectangular room needs. For an irregular room the
quickest source is a phone or tablet with a LiDAR scanner — the iPhone Pro models from the 12 Pro onward, and the iPad
Pro models since 2020 — running a room-scanning app: a slow walk around the room gives a floor plan with its dimensions
in a minute or two, accurate to a few centimetres, which is far finer than the model needs. Read the corner positions
off that plan and type or drag them in the planner, with the front wall at the top. The same scan gives you the
distances the planner asks for in step 2 — the fronts to the front wall, the seat to the speakers — which a measurement
cannot read. A plan drawn by hand from a tape measure works just as well; the planner wants the inner faces of the
walls, and a few centimetres of error change nothing.

**Name and files.** The planner keeps your current room between sessions by itself. *Save room…* writes it to a file
(the folder *Documents\GSonic Evo 32\rooms* is proposed) that you can open again or send to someone; *Open room…*
brings one back. Give the room a name in step 1 — it becomes the file's name.

## 4. Step 2 — seats and speakers

**The seats.** Place the main seat (x from the left wall, y from the front wall) and type your ear height while
seated. Choose the seating: one seat, two seats (1 m), a sofa (1.6 m) or a wide sofa (2.4 m). The planner judges the
bass across that width, not at one point — with a sofa, a second subwoofer's seat-to-seat benefit shows up; with a
single seat it cannot.

**The front speakers.** Drag them on the plan or type their positions; "keep L and R symmetric" mirrors them. Set the
crossover the receiver uses for the fronts, say whether their bass is a sealed box, ported or full range, and where
they are 3 dB down. Opened from a session, these come from your run.

**The subwoofers.** Tick the ones you have (up to four) and drag them on the plan or type their place. Their delay,
level and polarity are what a calibration would set — *Auto-align* finds them for the positions as drawn; you do not
tune them by hand.

**Placing the speakers from your measurement.** With a measured session the button *Place the speakers from my
measurement* puts the fronts where the measurement heard them. One thing to know: a cluster of microphone positions
measures every speaker's direction exactly, but not how far away things are. The planner therefore asks for your tape
measure — any of *seat to FL*, *L to R* and *fronts to front wall* scales the measured layout, several are averaged,
and the note under the fields shows what the layout then implies for all three. If your numbers disagree with each
other by more than a few percent, the note says so rather than hiding it; usually the seat is drawn in the wrong place.

**Heights are yours to measure.** The measurement cannot read how high a speaker sits. Both fronts stand at one
height: the tweeter height if you type it, otherwise your ear height (in most rooms the two are close).

## 5. Step 3 — finding the best spots

**The map.** *Find the best spot* scores every practical position for the chosen subwoofer and paints the floor: bright
means flatter bass across your seats, dark means rougher, hatched means not searched. The five best spots at least
0.9 m apart are numbered on the plan and listed with their flatness and the gain against the present spot; *Move it
here* moves the subwoofer there with the settings found for it.

**Practical positions.** By default a subwoofer goes within 0.8 m of a wall and at least 1 m from every seat. Both are
checkboxes. Untick "only near the walls" to let the search cover the whole floor; untick "keep 1 m from the seats" if a
subwoofer beside the sofa is a real option for you.

**Several subwoofers.** With more than one subwoofer ticked, every candidate position is judged with *every*
subwoofer's delay, polarity and level re-aligned around it — the map for subwoofer 2 depends on where subwoofer 1
stands, as it should. *Find the best arrangement* moves all of them at once: every combination of the practical
positions is tried with the subwoofers aligned — seconds for two subwoofers, minutes for three, and for four a quick
pass over a coarser grid first, with a thorough search offered after it and its time estimate (measured on your own
machine) shown before it starts. It can be stopped at any time and keeps what it found. The three best arrangements are
listed with every subwoofer's settings, drawn on the plan as you hover over them, and applied with one click (*Use
it*). Two subwoofers are never placed within 0.9 m of each other.

**What the score means.** The planner judges every spot twice: once at the damping that matches your room best, and
once at three times that decay, and ranks it by the worse of the two. A spot has to be good under both pictures of the
room. Hovering a spot shows both numbers. Differences under about 1 dB between spots or arrangements are inside the
model's own uncertainty — treat such spots as equals and pick the practical one.

**Let the level change.** Ticked, the alignment may set each subwoofer's level as well as its delay and polarity
(centred on the level that matches it to the fronts across the crossover). Unticked, the levels stay as typed.

## 6. The measurement check — how far to trust the map in your room

This is the planner's honest confidence indicator, and the reason to open it from a measured session.

Put the subwoofer on the plan where it stood when you measured, choose which measured subwoofer it is and which drawn
subwoofer it corresponds to, and press *Check the model*. The planner reads the subwoofer sweep your calibration recorded at the microphone positions, compares it with
its own prediction at your seats between 40 and 100 Hz, tries a range of room dampings and keeps the best fit, draws
the measured curve on the chart as a dotted line, and gives one of three verdicts:

- **good** — the model follows your measurement to within about 2.5 dB: the map can be trusted for ordering positions.
- **fair** — within about 4 dB: trust large differences between spots, not small ones.
- **poor** — the model and the room disagree: treat the map as a sketch and let the measurement decide.

Two things to know about the check:

- The damping it settles on is short — shorter than a room's real bass decay. That is expected: the shortest damping
  blurs the model's modes until its misplaced detail stops hurting, and it is the blur that fits best. The planner
  compensates by also judging every spot at three times that decay (see "What the score means").
- The verdict belongs to the room *as drawn*. If the fit is poor, check the outline and the seat position first — the
  check is also a test of your drawing. A very leaky room (open plan, light walls, large openings) will read fair or
  poor however well it is drawn; that is the model's limit, not a fault in your measurement.

On the rooms the model was checked against so far it followed the measured subwoofer sweep to about 2 dB rms over
40–100 Hz. In one of them a subwoofer had been measured both at its wall position and at a spot beside the seat that
an earlier version had suggested; the model reproduced, within about 2 dB, the 12 dB of deep bass that near-seat spot
lost, and ranked the wall position above it — which is what the listener heard.

## 7. Reading the chart and the maps

**The response chart** shows the model's prediction at the seat: the fronts, each subwoofer, and the sum, with the
seat-to-seat spread as a shaded band when the seating is wider than one seat, and the measured sweep as a dotted line
after a check. The scored band (20 Hz to 1.5 × the crossover, at least 100 Hz) is shaded; above it the model is
decoration. The smoothing selector beside the legend (none, 1/24, 1/12, 1/6 or 1/3 octave) changes only what is drawn —
the scoring stays unsmoothed, and the check compares at 1/6 octave on both sides.

**The pressure map** paints the room at one frequency: where a mode is loud and where it is quiet. Step through the
room's modes with the arrows, or click a mode in the *Room modes* list (every mode below 200 Hz, with its frequency)
to see its pattern. A seat in a mode's quiet zone will have a hole there that no subwoofer position fully fills; a
subwoofer in a mode's loud zone drives that mode hardest.

## 8. Advanced settings

Most users never need these; the defaults are the calibration's own conventions.

- **RT60 at bass** — the room's damping in the model. The measurement check sets it for you. By hand it is the
  model's blur: a shorter value sharpens the modes, a longer one smears them. It is not a measured reverberation
  time, and the check's value is usually shorter than a room's real bass decay (see section 6).
- **Pressure zone** — how the room behaves below its lowest mode: leaky (typical), sealed room, or none.
- **Air temperature** — sets the speed of sound.
- **Plot to** — the chart's upper frequency.
- **Scored band** — placement (20 Hz to 1.5 × the crossover, at least 100 Hz; the default) or wide (20 Hz to 2 × the
  crossover, at least 200 Hz). The default is the band where a subwoofer's position acts and where the model holds.
- **Sub low-pass / speaker high-pass** — the crossover filters' slopes: by default the receiver's 24 dB/octave
  low-pass to the subwoofers (LR4) and its 12 dB/octave high-pass on the speakers (BW2).
- **Mains delay / level** — offsets for the fronts, if you want to explore them.
- **Setup text** — the whole setup as text, to copy and paste between machines.

## 9. Questions

**Does it change my calibration?** No. Nothing in the planner touches a run, a filter or the receiver. Only a new
measurement and a new run change your calibration.

**Do I need a measurement to use it?** No — draw a room and play. With a measured session you get two things more: the
speakers placed from the measurement, and the check that tells you how far to trust the map in your room.

**Why does the sub's drawn position matter for the check?** The check compares the sweep recorded at one real position
with the model at that same position. Put the subwoofer where it stood when you measured, then move it afterwards.

**The planner says my best spot is beside the sofa.** With "keep 1 m from the seats" unticked, the near-field spot is
often the model's literal optimum. It is a real option if you can live with a subwoofer there; otherwise leave the rule
on and read the near-wall shortlist.

**Two spots differ by 0.3 dB. Which one?** Neither, by the model. Pick the practical one, or the one that measures
better.

**How accurate is it?** A few dB, less above 100 Hz, and the measurement check tells you for your room. It is a model
of a rigid rectangular-walled space with one damping value — good enough to order positions in rooms where the check
reads good, a sketch where it reads poor.

**Can it place the centre or the surround speakers?** No. The other speakers are drawn for orientation only; the
planner's physics is the subwoofers' and the fronts' bass.

**Where should the seat go?** The planner answers for the subwoofers with the seat where you put it. You can move the
seat and search again to compare seating positions by hand.

**I use the REW room simulator before placing subwoofers. How does this differ?** Both are models of a room's modes.
The planner takes any floor outline, not only a rectangle; it sets each subwoofer's delay, level and polarity itself for
every candidate position, as a calibration would, instead of leaving them to you; it searches all two to four
subwoofers' positions together; it judges each spot under two dampings and ranks by the worse; and, opened from a
measured session, it checks its own model against the subwoofer sweep your calibration recorded and tells you how far
to trust it. It is narrower in other ways: no per-wall absorption, no furniture, nothing above the bass. Use whichever
you trust more for a first guess — and let the measurement decide.

---

*The Room Planner is experimental. If a move makes the calibration worse, move back.*
