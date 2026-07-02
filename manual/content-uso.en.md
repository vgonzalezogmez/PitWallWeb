# User manual — PitWall (organization / race direction)

A guide for whoever **operates** PitWall: setting up the race, running it live, fixing laps and producing results.

---

## 1. Introduction
![img: 01-home.png]

**PitWall** is the timing and management system for slot racing. It detects each car crossing the finish line through the timing hardware, with two compatible options:

- **DS-300** — via **serial port**. You can combine **up to 6 DS-300 tracks** in a single race: each box times its own lanes and PitWall combines them.
- **BART (Policar)** — via **Bluetooth**. It supports **up to the maximum number of lanes that BART allows** (currently **32**).

You can use either source; for PitWall the flow of crossings is equivalent.

- From the **home screen** you reach **Races**, **Settings** and the rest of the modules.
- At the bottom right you always see the **link status** (green = connected; "Sin señal" / no signal = check the cable/port or the Bluetooth).

**The race list** shows all your races with their status (pending / active / finished) and the New race (“+ Nueva carrera”) button.

![img: 02-races-list.png]

## 2. Scenarios, categories and catalogs (your library)

To avoid reconfiguring the same thing for every race, PitWall keeps **reusable templates** that you then pick when creating a race.

**Scenarios (saved tracks).** A **scenario** is a saved physical track: number of tracks and lanes (e.g. `8+8+8 = 24`), its **lane sequence** (rotation) and the **default minimum time**. Any race assigned to that scenario inherits everything automatically.

![img: op-escenarios.png]

When editing a scenario you define its name, the lane configuration, you drag the **rotation sequence** (with **DSC rests** if there are spare drivers), the **default minimum time** and, optionally, **minimum laps per category** (a different Pt for GT, Touring, Classics… on that same track).

![img: op-escenario-form.png]

**Categories.** Level/class groups (GT, Touring, Classics…) that serve to **override the minimum time (Pt) per category** in each scenario and to classify cars and drivers.

![img: op-categorias.png]

**Reusable catalogs (drivers, teams, cars).** Keep your **database** of participants and equipment to reuse it across races:
- **Drivers** — name and category; each driver can have their identification **QR**.
- **Teams** — name, color, country, car and members.
- **Cars** — make, model and category.

All of them can be **bulk-imported from CSV** (the CSV template (“Plantilla CSV”) and Import CSV (“Importar CSV”) buttons, with a preview of new entries vs. duplicates) and exported.

![img: op-catalogo-pilotos.png]

![img: op-qr-pilotos.png]

> With Export QR (“Exportar QR”) you print the QR cards for all drivers (for the scan-based driver change in endurance — see *Driver shift control*).

## 3. Creating a race
![img: 03-wizard-step1.png]

Press New race (“+ Nueva carrera”) and follow the wizard:

- **Type**:
  - *Sprint* → a **quick race**, of **drivers or teams**.
  - *Endurance* → an **endurance race** (by teams), which adds the **control of how much each driver of the team has run** (see *Driver shift control*).
- **Lanes and tracks**: total number of lanes and how they are split across boxes (e.g. 8+8+6 = 3 DS-300 boxes).
- **Minimum lap time (Pt)**: below this time, a crossing is considered a **ghost** (bounce/double read) and does not count.
- **Passes**: how many times the **entire lane sequence** is run. 2 passes = the full rotation is run twice (double the heats).
- **Repeat lane**: each lane is run this number of **consecutive heats** (same lane), adding up the laps — to compare each repetition.
- **Pole** (optional) and **driver rules** (championship only: min/max per driver, change lock at the end of a heat).

> **Passes** and **repeat lane** only change how the heats are generated; totals are summed per participant.

## 4. Batches, participants and rotation
![img: 34-tanda.png]

A **batch** groups the participants and their **lane rotation** per heat. When you add the **teams/drivers**, PitWall automatically generates all the **heats**.

**How rotation works.** Each participant keeps changing lanes from heat to heat following the configured sequence (e.g. `1, 3, 5, 6, 4, 2`). This way everyone goes through every lane and conditions are evened out.

- *Example (6 lanes, 6 drivers):* in heat 1 driver A runs lane 1; in heat 2, lane 3; in heat 3, lane 5… until completing the loop through all lanes.

**Rotation your way.** PitWall proposes a balanced rotation automatically, but **you can manage it however you like**: reorder the **lane sequence** by hand (by dragging) to decide exactly which lane each participant runs in each heat.

**Rests.** If there are **more participants than lanes**, the sequence includes gaps (`0` / `DSC`) that are **rests**: in that heat that participant does not run. PitWall spreads them out evenly, but **you can also place them wherever you want** within the rotation (drag them to the position you prefer).

**With passes / repeat lane:**
- *2 passes* → the whole sequence repeats: `1,3,5,6,4,2, 1,3,5,6,4,2`.
- *Repeat lane 2* → each lane, two consecutive heats: `1,1,3,3,5,5,6,6,4,4,2,2`.

## 5. Editing race, batches and heats

After creating a race you can tweak it:
- **Edit race** — change the **name** and, if it **still has no laps recorded**, the track/scenario. If there are already laps, the track is **locked** (so as not to break the data).

![img: op-edit-carrera.png]

- **Edit batch** — change the **names** of the participants and, if the batch hasn't started yet, its composition. If it already has heats started, it enters **rename-only mode** (no participants added or removed, so as not to unbalance the rotation).

![img: op-edit-tanda.png]

- **Edit heat** — change **who runs in each lane** in a specific heat, without regenerating the whole batch (useful if a team doesn't show up or there's a last-minute change).

## 6. Pole (pre-race qualifying)
![img: 44-pole-setup.png]

The **pole** is a qualifying lap **before** the race to decide the starting order. It's optional; it's enabled when creating the race (**Pole**) and it's launched from the race page → Set up Pole Position (“Configurar Pole Position”).

- **Participants**: everyone entered appears. The **order of the list** is the order in which they'll go out to do their lap; hit 🎲 Random (“🎲 Aleatorio”) to shuffle it.
- **Pole lane**: **everyone** does their qualifying lap on the **same lane** (so it's comparable). Pick it with **−/+** or with 🎲 Random (“🎲 Aleatorio”).
- Press Start Pole (“Empezar Pole”): each participant enters in turn, does their lap and PitWall records their best time. In timing you can enable Skip 1st crossing (“Omitir 1er cruce”) (out-lap) so the launch lap isn't counted.

**Pole results.** When it finishes, Pole Results (“Resultados Pole”) appears with the **final classification** (from fastest to slowest, with the gap to the leader and the **fastest lap**). From here you can ✏️ Edit times (“✏️ Editar tiempos”) if there was an error, or continue with 🚦 Assign starting lanes (“🚦 Asignar carriles de salida”).

![img: 46-pole-results.png]

**Assigning lanes after the pole.** The pole doesn't distribute lanes automatically: it opens the Lane choice (“Elección de carril”) screen, where each participant **chooses** their lane **in classification order** — the **poleman** (the fastest) chooses first, then the 2nd, and so on. It's the classic "the fastest one picks lane".

![img: 47-pole-lanes.png]

- The Choosing now (“Eligiendo ahora”) banner indicates whose turn it is; on the left you see the **choosing order** (the classification) and on the right the **available lanes** (with their color).
- Each one presses the lane they want; that lane disappears from the available ones and the turn passes to the next.
- **If there are more participants than lanes**, 💤 Rest (“💤 Descanso”) gaps appear: whoever picks a rest **doesn't run heat 1** and **enters the rotation from heat 2**.
- When everyone has chosen, press 🏁 Create First Batch (“🏁 Crear Primera Tanda”): PitWall creates the batch and generates all the heats with that grid as the starting point (the choosing order defines the initial position in the lane rotation). From there, the race rotates the lanes heat to heat as always (see *Batches and rotation*).

> The pole doesn't score in the race: it only decides **who picks lane first** and, with that, the starting grid of the first heat.

## 7. PitWall Lap — PIN for the teams
![img: 43-lap-pins.png]

**PitWall Lap** is the mobile view for each **team/driver** to follow their own timing from the phone (their laps, called out by voice, and their position). So that they only enter *their* panel, a **PIN** is handed out per team.

- Go into PitWall Lap · PINs (“PitWall Lap · PINs”) of the race. You'll see the address teams open on the mobile (e.g. `http://<server-IP>:3000/lap/<id>`) and the **TEAM → PIN** table.
- Give each team **their PIN**. When they open the address and enter it, they go straight into their panel.
- New (“Nuevo”) regenerates a team's PIN (in case it was leaked or they want to change it).

> The phones must be on the **same network** as the computer acting as server. Use the computer's IP, not `localhost`, when they open it from the phone.

## 8. Running the race live
![img: 20-live-timing.png]

From the race page:

1. **Arm the heat** (▶). It stays ready waiting for the **GO** from the box.
2. **GO**: when the start is given at the box, the **lights** appear and the timer starts. Each track has its own clock (C1/C2/C3).
3. During the heat you see per lane: **total laps**, **last**, **average**, **best**, and at the top the **fastest lap** banner.
4. **Pause / Resume / Stop** the heat when needed.
5. When it ends (flag or time out), the heat closes and the **next one** is prepared.
6. When all the heats of a batch are done, the **next batch** starts.

**Choosing the view.** With the View (“Vista”) button you change the layout depending on the lanes: *Horizontal rows* (few lanes), *Compact grid* (many) or *Cards with details* (with laps/exits/pit/Δ per card).

**Switching batch, repeating a heat and finishing.** From the live screen itself you have shortcuts without leaving the screen:
- **Next batch** — when a batch's heats are done, it moves straight to the next.
- **Repeat heat** — if a heat was called bad (false start, incident), you launch it again with the same participants and lanes.
- **Finish race** — closes the race (the "flag"): the classification is frozen and the summary is generated for results and for the mobiles (PitWall Lap).

> "Sin señal del DS-300" (no DS-300 signal) warning: while it's showing, laps are **not recorded**. Check the connection before giving the GO.

## 9. Driver shift control (championships)

In **team championship** races you can enforce rules for sharing the wheel among a team's drivers. They are defined when creating the race:
- **Minimum / maximum time per driver** — each driver must run at least X and at most Y.
- **Lock after a change** — a minimum time before changing driver again.
- **Maximum number of shifts per driver**.

**Driver changes** are recorded by scanning the **driver's QR** (or entering their code) when they come onto the track. From the live screen you open **Shift control**, which shows the **current driver per lane**, the **accumulated time** of each one (warning if they break a rule) and the **shift history**; if a change was recorded wrong, you can **correct the time** of the shift.

## 10. Lap by lap and corrections (add / remove laps)
![img: 30-correcciones.png]

From the race (the **lap correction** button in the live screen or in results) you enter the **lap by lap** of each heat. It serves to fix wrongly recorded readings.

- **Left**: the lanes of the heat; pick the team/driver to review.
- **Right**: their lap list — **LAP** (no.), **TIME**, **CLOCK** (race moment) and **Δ PREV.** (difference from the previous lap).
- **Actions per lap**:
  - **Transfer** (↔) — pass the lap to **another lane/team** (if the system assigned it wrong).
  - **Ghost** — mark the lap as invalid (doesn't count) without deleting it; it can be **restored**.
  - **Delete** (🗑) — remove a lap.
  - **Add manual lap** — if a crossing was missed, you add it by hand.

> Use it with judgment: corrections change totals, averages and classification of that heat.

## 11. Results and exports
![img: 10-results-comparativa.png]

When it finishes (or at any time) go into **Results**:

- **Comparison** (grid): per participant, each lane with **Fastest / Average / Consistency / Exits / Pit-stops**. In **passes/repeat-lane** races, each lane is broken down into its **occurrences** (1/2, 2/2) to compare.
- **Progression / Positions / Gap to leader / Gap (grid) / Advanced statistics**: different analysis views (explained in detail in the *Statistics manual*).
- **Exports**: **Excel**, **Points (xlsx/csv)**, **Control (csv)**, **Export for GitHub**, **PDF**.

**Public results.** There's an open page —**Results**, in the home menu— where anyone can consult (without touching anything or being able to edit) the results of the **finished** races. It's the one you share with drivers and public so they can look at the classification and statistics of the race.

![img: op-resultados-publicos.png]

## 12. Training
![img: 40-training.png]

Besides races, PitWall has a **Training** mode (from the home screen) to run without setting up a full competition. There are two modes:

- **Free training**: records **laps per lane without a team structure**. Ideal for open sessions where each person tries the car and track; there's no rotation or classification, just times per lane.
- **Competition**: teams or drivers assigned to lanes with **automatic rotation after each batch**, like a race but designed to practice the championship format.

Choose the mode, assign the lanes and press **Start**. Live timing works the same as in a race (box GO, laps, best/average per lane).

## 13. Settings
![img: 04-settings.png]

- **Hardware / ports**: configure the serial tracks (DS-300) and their number of lanes.
- **Tracks**: define saved tracks (lane sequence, minimum time).
- **License** and language (ES/EN).

## 14. Glossary (operation)
- **Race**: the complete event. Made up of batches.
- **Batch**: group of participants with their rotation; made up of heats.
- **Heat**: one timed run (all lanes at once) of a set duration.
- **Rotation**: how participants change lanes from one heat to another.
- **Rest**: a heat in which a participant doesn't run (a `0` gap in the sequence).
- **Pass**: a complete run through the lane sequence; N passes = N× heats.
- **Repeat lane**: run each lane N consecutive heats, adding up laps.
- **GO**: the start signal (from the DS-300 box) that launches the heat.
- **Ghost lap**: a lap marked as invalid (doesn't count), restorable.
- **Pole**: a pre-race qualifying session (optional); everyone runs on the same lane and their best lap sets the starting grid.
- **Free training**: mode to record laps per lane without teams or rotation (open session).
- **PitWall Lap**: per-team/driver mobile view (their called-out laps and their position).
- **PIN**: per-team code to enter their panel in PitWall Lap.
- **Pt (minimum time)**: threshold below which a lap is considered a ghost crossing and doesn't count.
- **Scenario**: a saved track (tracks, lanes, sequence and minimum time) reusable across several races.
- **Category**: a car/driver class (GT, Touring, Classics…); allows a different Pt per category.
- **Catalog**: reusable library of drivers, teams and cars (importable via CSV).
- **Driver QR**: a code that identifies the driver to record their shift when scanned.
- **Shift**: the period a driver is at the wheel within their team in endurance.
- **DS-300**: the timing box that detects the crossing at the line.
