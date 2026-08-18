# breakdown.md
This is a detailed breakdown of every scene in the visual novel,
including locations outfits etc etc.  The actual scenes will be
created using this file as a reference.

---

## How to read this

This breakdown is derived from the five route treatments in `wiki/treatment/`
(Ember, Isolde, Seraphine, Wren, and the dark **Undivided** / polygamy arc) and
the shared act skeleton in `wiki/outline.md`.

**Branch model.** All five routes share one trunk: the opening act and the early
part of act two are the *same* scenes for everyone, coloured only by which love
interest Caedon gravitates toward. The story then forks:

```
COMMON TRUNK (Act I + early Act II)
        │
        ├─ c11_execution  ← the stranded-pair execution beat = the fork
        │
        ├── romance branches (determined by accumulated affection):
        │     ├─ EMBER   (em_*)
        │     ├─ ISOLDE  (is_*)
        │     ├─ SERAPHINE (se_*)
        │     └─ WREN    (wr_*)
        │
        └── DARK BRANCH: "The Undivided" (ud_*)
              — taken when Caedon has committed to NO single love interest;
                it diverges AT c11_execution and never rejoins.
```

The four romance branches reuse every trunk scene verbatim; they differ only in
their act-two tail and act three, and each ends in a wedding. The dark branch is
foreshadowed from Act I by *how* Caedon plays the trunk (cataloguing rather than
courting), but only formally splits off at the execution beat, and ends in
conquest + a timeskip civil war, no wedding.

**Scene IDs.** `c##_*` = common trunk. `em_/is_/se_/wr_/ud_*` = per-route. IDs
are stable handles for the eventual `[[scene: ...]]` markers and
`[[choice:]]`/`[[next:]]` targets when these become `scenes/` chunks.

**Status of assets.** Today only `scenes/opening.md` and the 11 cast sheets
exist; the only location with any presence is `a_room` (mined, no sheet). Every
location named below still needs a sheet, and the branch scenes still need to be
written as `scenes/` chunks. See the Locations index and Cast index at the end,
which double as build checklists. `opening` is expected to become the pre-title /
title card that leads into `c01_arrival`.

---

# COMMON TRUNK

## Act I — The Intake

### c01_arrival — Arrival at the Cog-College
- **Location:** cog_college_approach (the gates / outer courtyard of the college)
- **Characters:** Caedon Vale; Headmistress Auria Coyle (welcoming the intake);
  the four love interests glimpsed in the crowd; Gideon Marsh, Pip Calloway,
  Tobias Renn among the cohort.
- **Summary:** Caedon arrives among a licensed, metered intake of talents.
  Establishes the world: Cog-College magic academy, the Weave, Governors and
  Ferran licensing, and the ever-present threat of Rust-scarring from ungoverned
  power. Headmistress Coyle frames the college's double mission — to train
  channelers and to police ungoverned ones. Caedon registers the four standout
  students without yet choosing among them. Sets the "gravitates toward a love
  interest" dial that will decide the route.

### c02_first_meetings — The four standouts
- **Location:** cog_college_courtyard / practice_yards
- **Characters:** Caedon; Ember Kellan, Isolde Vorn, Seraphine Halcyon,
  Wren Ashfield (each introduced in their element).
- **Summary:** Caedon crosses paths with each love interest and gets his first
  read on them — Ember channeling raw current in the yards where the cautious
  hang back, rust already blooming on her forearm; Isolde's aristocratic
  stillness and key-pendant, keeping ungoverned talent at arm's length;
  Seraphine at the centre of every room without seeming to seek it, ringed by
  envoys; Wren, the guarded scholarship outsider who slips the college's rules
  like weather. This is the hub where the player's attention begins to weight
  the route.

### c03_the_friend_group — Finding footing
- **Location:** dormitory_commons
- **Characters:** Caedon; Gideon Marsh, Pip Calloway, Tobias Renn.
- **Summary:** Caedon settles in with the other male students and the wider
  friend group. Lighter, character-building beat that establishes the ensemble
  who will crew the ruins test — and, later, become stranded pairs scattered
  across the world.

### c04_first_class — Weaves and the leash
- **Location:** lecture_hall
- **Characters:** Caedon; Professor Mirabel Quist; Professor Silas Thorn;
  the four love interests (contrasting channeling styles on display).
- **Summary:** First class establishes channeling technique and doctrine:
  metered vs. spent power, "Vash-strong" raw current (Ember, Wren) against
  "Sela-strong" precision (Isolde, Seraphine), and the fact that ungoverned
  channeling is a crime the college itself trains students to police. Caedon
  watches each love interest's signature: Ember refusing to meter, Isolde
  leashing herself tight, Seraphine braiding Spirit and Air with unnerving
  delicacy, Wren answering nothing she isn't forced to, her scarred hands gloved.

### c05_ruins_briefing — The field test
- **Location:** lecture_hall / assembly_hall
- **Characters:** Caedon; Headmistress Auria Coyle and/or Professor Quist;
  the friend group and the love interests.
- **Summary:** The cohort is assigned to investigate a set of ruins as a
  practical test. Stakes and teams are set. Seeds the dangers to come.

### c06_the_ruins — Into the ruins
- **Location:** the_ruins (exterior) → ruins_interior
- **Characters:** Caedon; the friend group; the four love interests.
- **Summary:** The team explores the ruins. Tension builds toward the ambush.
  (Route colour: on the Wren-leaning path the "nefarious actors" prove to be
  Grey Hand Assayers hunting a fugitive channeler who fled into these ruins,
  turning the test into a real escape.)

### c07_the_ambush — Nefarious actors intervene
- **Location:** ruins_interior
- **Characters:** Caedon; the friend group; the four love interests; the
  attackers (unnamed external actors / Assayers).
- **Summary:** Outside actors intervene and the test becomes real danger. This
  is the first showcase of each love interest under pressure, and which of them
  carries the fight foreshadows the route:
  - *Ember* spends power without counting the cost, saving the group but burning
    herself.
  - *Isolde's* disciplined precision wins where recklessness would fail — but
    forces her to break a rule she believes in.
  - *Seraphine* reads the ambush and talks/misdirects/weaves a losing fight into
    a win, and alone recognises it was arranged.
  - *Wren's* smuggling contacts (a cloudlane cache, a bolt-hole) are the only
    reason anyone gets out.
  - *(Undivided colour)* Caedon coordinates all four at once, each covering the
    others' weaknesses, and they win with unnerving efficiency.
  They emerge victorious.

### c08_aftermath — Drawn in
- **Location:** cog_college_courtyard / infirmary
- **Characters:** Caedon; the love interest(s); friend group.
- **Summary:** In the aftermath Caedon is pulled into the conflict surrounding
  the love interest he's drawn to — the Dominion's proprietary claim on Ember and
  the Ferran distrust of ungoverned Vash strength; Vorn's watchers and the
  Assayers' reach around Isolde; the rival houses and treaty intrigue around
  Seraphine; the Assayer hunt for the unlicensed and the Ashen Circle around
  Wren. On the Undivided colour, he is drawn into *all four* conflicts at once and
  refuses to pick a side or a heart.

## Act II — The World Breaks (shared setup)

### c09_woods_training — Training in the woods
- **Location:** college_woods
- **Characters:** Caedon; the love interest (romance branches) — or Caedon alone
  (Undivided colour).
- **Summary:** The intimate turn. On a romance path this is the first thing that
  is truly *theirs*: Ember teaches Caedon to spend rather than meter; Isolde
  confides the doubt beneath her devotion; Seraphine and Caedon learn to read
  each other's threads; Wren teaches smugglers' cloudlane craft. On the Undivided
  colour Caedon trains *alone*, hardening himself — building a self, not a bond.

### c10_the_world_breaks — Intensified training / the crisis
- **Location:** assembly_hall / practice_yards
- **Characters:** Caedon; Headmistress Auria Coyle; professors; the whole cohort.
- **Summary:** Something goes catastrophically wrong on the geopolitical scale.
  The college intensifies training as the situation worsens. Dread and urgency.

### c11a_teleport — Scattered in pairs
- **Location:** teleportation_hall → (destination varies by route)
- **Characters:** Caedon; the paired love interest; cohort dispersing.
- **Summary:** As things deteriorate, the school teleports the students out in
  pairs to random places around the world to scatter them beyond reach. Caedon
  lands with his love interest (romance branches). The destination is the
  route's foreign locale.

### c11b_on_the_run — Hunted
- **Location:** route-specific (see branches)
- **Characters:** Caedon; the love interest.
- **Summary:** On the run from hostile security services. The love interest's
  particular competence keeps them alive (Ember's raw power as shield-and-beacon;
  Isolde's Assayer knowledge and Vorn devotional networks + key-pendant;
  Seraphine's court protocol and cipher; Wren's smuggler underground). Together
  they piece together the truth behind the world's collapse.

### c11_execution — THE FORK: the executed pair
- **Location:** a public square / broadcast (route-specific dressing)
- **Characters:** Caedon; the love interest; (offscreen) another stranded pair.
- **Summary:** Word reaches them — or they witness — that another stranded pair,
  fleeing in a neighbouring country, was caught, interrogated, and publicly
  executed. **This is the branch point.**
  - On a **romance route**, the atrocity lands as grief and resolve, hardening
    the love interest and pushing the pair from surviving to acting.
  - On the **Undivided route**, Caedon sees or learns the full brutality of it in
    detail the other routes spare him; it *breaks* something in him. Having given
    his heart to no one, he vows to lose *none* of them — the refusal to choose
    becomes a refusal to lose. → go to `ud_*`.

---

# ROMANCE BRANCH — EMBER KELLAN (em_*)
*Throughline: raw ungoverned Vash power vs. Ferran licensing, under the shadow of
the Rust. A romance lived under a sentence.*

### em_landing — Far from any forge
- **Location:** vashan_borderland (open country, no forge to shelter her kind)
- **Characters:** Caedon; Ember Kellan.
- **Summary:** They land far from any forge that would shelter Kiln-Sworn. Ember's
  raw power is both shield and beacon — it saves them from pursuit and draws more
  of it. Between escapes she lets slip, never as complaint, how little time she
  believes the Rust will leave her; the executed pair lands on Caedon as a warning
  about her.

### em_alliances — The Kiln-Sworn open doors
- **Location:** vashan_forge_city (Vashan Dominion)
- **Characters:** Caedon; Ember Kellan; Kiln-Sworn contacts; surviving stranded
  pairs (offscreen/liaison).
- **Summary:** Ember's Kiln-Sworn ties and forge-craft open Dominion doors no
  licensed talent could. Caedon exposes corruption at the highest levels while
  Ember arms and equips their growing coalition. Some stranded pairs murder the
  monarchs of their landing-nations; others build comms back to Caedon.

### em_infiltration — The Rust creeps
- **Location:** enemy_organization_approach / battlefronts
- **Characters:** Caedon; Ember Kellan; recruited allies; surviving pairs.
- **Summary:** They infiltrate the organization behind the chaos across several
  battles. Ember spends her strength recklessly in each; the Rust climbs further
  up her arm — the cost of every victory written on her body. Caedon's fight
  becomes as much against her fatalism as against the enemy.

### em_final_boss — The final assault
- **Location:** enemy_organization_core
- **Characters:** Caedon; Ember Kellan; allies; surviving pairs.
- **Summary:** The converged coalition storms the boss. The boss falls. Ember
  lives.

### em_ending — Long is possible
- **Location:** vashan_forge_city (wedding)
- **Characters:** Caedon; Ember Kellan.
- **Summary:** Marrying Ember is Caedon's argument, made in deed, against the
  sentence she's carried her whole life — she loved fiercely because she never
  expected to love long; he stays to prove long is possible. The end.

---

# ROMANCE BRANCH — ISOLDE VORN (is_*)
*Throughline: doubt against devotion. Cold Sela precision unclasped from the
piety that leashes it, until she chooses her own thread.*

### is_landing — On the run from her own
- **Location:** vorn_environs (the Grey Principality of Vorn / Assayer country)
- **Characters:** Caedon; Isolde Vorn.
- **Summary:** They land where Isolde's knowledge cuts both ways. Her grasp of
  Assayer methods and Vorn devotional networks keeps them alive; her key-pendant
  opens doors it should not. They uncover the truth — and it implicates the very
  order Isolde was raised to serve. The executed pair lands on her like a verdict
  on her own faith.

### is_alliances — Faith turned on its makers
- **Location:** vorn_stronghold / devout government halls
- **Characters:** Caedon; Isolde Vorn; surviving stranded pairs (liaison).
- **Summary:** Isolde's faith becomes a weapon turned on its makers: she exposes
  corruption at the highest levels of the devout governments and the Assayer
  hierarchy, while Caedon exposes corruption broadly. Some pairs assassinate their
  landing-nations' rulers; others open comms back to Caedon.

### is_infiltration — The knife drawn
- **Location:** enemy_organization_approach / battlefronts
- **Characters:** Caedon; Isolde Vorn; recruited allies; surviving pairs.
- **Summary:** They infiltrate the organization behind the chaos, fighting
  several battles. Isolde, at last, draws her hidden knife of doubt in the open
  and chooses her own thread rather than the leash of her province.

### is_final_boss — The converged fight
- **Location:** enemy_organization_core
- **Characters:** Caedon; Isolde Vorn; allies; surviving pairs.
- **Summary:** Recruited allies and surviving pairs converge for the final fight;
  the boss falls.

### is_ending — Her own thread
- **Location:** vorn_environs (wedding)
- **Characters:** Caedon; Isolde Vorn.
- **Summary:** Caedon marries Isolde, who has unclasped her armour and chosen for
  herself. The end.

---

# ROMANCE BRANCH — SERAPHINE HALCYON (se_*)
*Throughline: the peace-broker's daughter choosing her own thread instead of the
one spun for her — and discovering the courts are complicit.*

### se_landing — Inside a foreign court
- **Location:** foreign_court (where her name is both shield and target)
- **Characters:** Caedon; Seraphine Halcyon.
- **Summary:** They land inside a foreign court. On the run from security
  services, they survive on Seraphine's fluency in court protocol and cipher —
  she opens sealed doors with a phrase and reads a room's true allegiances at a
  glance. Working the diplomatic underlayer, they uncover the truth: a
  coordinated design masked as coincidence, treaties written to concentrate
  control of the Weave. The executed pair hardens her: she stops believing she
  can broker her way out.

### se_alliances — Scandal into coalition
- **Location:** halcyon_reach / court chambers
- **Characters:** Caedon; Seraphine Halcyon; surviving stranded pairs (liaison).
- **Summary:** Seraphine's blood and bearing open doors closed to everyone else.
  Caedon exposes corruption; she weaves the fallout into alliances — scandal into
  leverage, leverage into a coalition. Some pairs murder their landing-nations'
  monarchs; others build comms back to Caedon, and she braids them into one front.

### se_infiltration — Courts turned
- **Location:** enemy_organization_approach / battlefronts
- **Characters:** Caedon; Seraphine Halcyon; recruited allies; surviving pairs.
- **Summary:** Together they infiltrate the organization behind the chaos,
  fighting several battles as the allies she brokered and the surviving pairs
  converge. She wins not by force alone but by turning the enemy's own courts
  against it.

### se_final_boss — The final fight
- **Location:** enemy_organization_core
- **Characters:** Caedon; Seraphine Halcyon; allies; surviving pairs.
- **Summary:** The converged coalition brings down the boss.

### se_ending — Chosen, not spun
- **Location:** halcyon_reach (wedding)
- **Characters:** Caedon; Seraphine Halcyon.
- **Summary:** Caedon marries Seraphine, who at last chose her own thread rather
  than the one spun for her. The end.

---

# ROMANCE BRANCH — WREN ASHFIELD (wr_*)
*Throughline: trust extended to someone who has never been able to afford it —
can she believe he will not sell her.*

### wr_landing — Shot on sight
- **Location:** hostile_border (territory where her kind are shot on sight)
- **Characters:** Caedon; Wren Ashfield.
- **Summary:** They land in hostile territory where Wren's scars mark her
  instantly. The roles invert: it's her underground, not Caedon's schooling, that
  keeps them alive — bolt-holes, forged tokens, smuggler debts called in.

### wr_truth — The harvest
- **Location:** cloudlane_bolthole / fugitive networks
- **Characters:** Caedon; Wren Ashfield.
- **Summary:** Threading the fugitive networks, they piece together the truth:
  it's bound up in the Assayers' program of mass severing — the severed aren't
  merely policed but *harvested*. The executed pair lands hard: exactly the fate
  Wren has run from all her life, made real for someone they knew.

### wr_alliances — The discarded
- **Location:** ashen_circle_haven
- **Characters:** Caedon; Wren Ashfield; the Ashen Circle; surviving stranded
  pairs (liaison).
- **Summary:** With the surviving pairs they build a coalition. Wren's value is
  singular: she opens doors among the discarded and the smuggler-nets no monarch
  commands. Caedon exposes corruption at the highest levels, feeding evidence into
  the networks Wren threads. Some pairs assassinate rulers; others open comms.

### wr_infiltration — Set-pieces
- **Location:** enemy_organization_approach / battlefronts
- **Characters:** Caedon; Wren Ashfield; the Ashen Circle; recruited allies;
  surviving pairs.
- **Summary:** With the Ashen Circle at their backs they infiltrate the
  organization behind the chaos, fighting through several set-piece battles.

### wr_final_boss — The discarded rise
- **Location:** enemy_organization_core
- **Characters:** Caedon; Wren Ashfield; allies; surviving pairs.
- **Summary:** The recruited allies and surviving pairs converge for the final
  assault — and the discarded, the people the world threw away, are the ones who
  bring it down.

### wr_ending — Trusted, wholly
- **Location:** ashen_circle_haven (wedding)
- **Characters:** Caedon; Wren Ashfield.
- **Summary:** Caedon marries Wren, and for the first time she is trusted, wholly,
  by someone who never sold her. The end.

---

# DARK BRANCH — THE UNDIVIDED (ud_*)
*Diverges at `c11_execution`. Love as instrument: refusal to choose becomes
refusal to lose, and refusal to lose becomes tyranny. No wedding.*

> Foreshadowing across the trunk (played as the "Undivided colour" above): in
> Act I Caedon commits to no one, keeping all four at a careful distance while
> letting each feel seen; in class he *catalogues* their strengths as assets, not
> as a suitor; at `c07_the_ambush` he conducts all four at once; at
> `c09_woods_training` he trains alone, hardening rather than bonding.

### ud_break — The break
- **Location:** (the execution locale — witnessed in full)
- **Characters:** Caedon (alone at this beat).
- **Summary:** Caedon witnesses or learns the full brutality of the stranded
  pair's execution, in detail the romance routes spare him. It breaks something in
  him. Having given his heart to no one, he vows to lose *none* of them, and that
  the world which killed them will answer. He no longer hunts the truth to
  survive — he hunts it to punish.

### ud_binding — Reunion in vengeance
- **Location:** scattered locales (Wren's smuggler-nets, Vorn, courts, Vashan
  forge) → a consolidating base
- **Characters:** Caedon; Wren, Isolde, Seraphine, Ember (reunited one by one).
- **Summary:** Caedon reunites with the love interests one at a time, binding each
  to him through shared vengeance and the promise that he can keep them all alive
  where the world could not. Wren opens the smuggler-nets, Isolde turns her Assayer
  knowledge inward, Seraphine reads the courts, Ember arms them. All four come to
  love him — and, for the first time, he lets himself love all four. It is
  genuine, which is what makes it dangerous: his love is total, so his vengeance
  is total.

### ud_conquest — The warlord
- **Location:** conquered_empire (nations destabilised and seized)
- **Characters:** Caedon; the four consorts; absorbed armies; slain rulers.
- **Summary:** Caedon and the four seek alliances but he uses them ruthlessly. He
  exposes corruption not to reform nations but to destabilise and seize them.
  Where the romance routes' pairs murder monarchs out of desperation, he kills
  them as conquest, absorbing their forces into a growing host. Coalition-building
  becomes empire-building; he bloodily conquers one empire and crowns himself and
  his four consorts over its ashes.

### ud_final_boss — A single monstrous working
- **Location:** enemy_organization_core
- **Characters:** Caedon; Isolde, Ember, Seraphine, Wren (the four instruments);
  the enemy.
- **Summary:** Caedon develops and deploys strategic-class weaves — weapons on the
  order of nukes — to utterly destroy the organization behind the chaos. Isolde's
  precision aims them, Ember's raw current powers them, Seraphine's braided
  subtlety hides them, Wren's forbidden craft smuggles them into place: the four
  assets he catalogued in Act One turned to one working. The boss falls — not to a
  hero but to a warlord. There is no wedding; there is a dynasty.

### ud_epilogue — The timeskip
- **Location:** ruined_cities (years later)
- **Characters:** Caedon (aged); his many children by all four consorts.
- **Summary:** Years later, Caedon's many children — born to all four consorts —
  fight a bloody civil war over his inheritance. The strategic weaves he pioneered
  are turned on cities. The world he conquered to protect the people he loved is
  left in ruins by the very children of that love: the harem fantasy followed to
  its logical, catastrophic end. The end.

---

# Locations index
*(build checklist — none have sheets yet except the mined `a_room`)*

**Common trunk / Cog-College:**
- `cog_college_approach` — the gates and outer approach (c01)
- `cog_college_courtyard` — main courtyard hub (c02, c08)
- `practice_yards` — open channeling yards (c02, c10)
- `dormitory_commons` — student common room (c03)
- `lecture_hall` — classroom (c04, c05)
- `assembly_hall` — briefings / crisis address (c05, c10)
- `the_ruins` (exterior) + `ruins_interior` — the field-test site (c06, c07)
- `infirmary` — aftermath (c08)
- `college_woods` — woodland training ground (c09)
- `teleportation_hall` — departure point of the paired teleport (c11a)

**Ember branch:** `vashan_borderland`, `vashan_forge_city`
**Isolde branch:** `vorn_environs`, `vorn_stronghold`
**Seraphine branch:** `foreign_court`, `halcyon_reach`
**Wren branch:** `hostile_border`, `cloudlane_bolthole`, `ashen_circle_haven`
**Shared endgame:** `enemy_organization_approach`, `enemy_organization_core`
**Dark branch only:** `conquered_empire`, `ruined_cities`

> Note: several trunk locations (ruins, woods, foreign locales) are the kind that
> `INT./EXT.` scene headings will mine automatically once the scenes are written;
> still, each should get a real location sheet for palette/mood/lighting control.

# Cast index
*(all 11 have draft sheets already)*

- **Caedon Vale** — protagonist; in every scene.
- **Ember Kellan** — love interest; Ember branch + Undivided consort.
- **Isolde Vorn** — love interest; Isolde branch + Undivided consort.
- **Seraphine Halcyon** — love interest; Seraphine branch + Undivided consort.
- **Wren Ashfield** — love interest; Wren branch + Undivided consort.
- **Gideon Marsh** — friend group / cohort (c01, c03, c06–c07); potential
  stranded-pair member.
- **Pip Calloway** — friend group / cohort (c01, c03, c06–c07); potential
  stranded-pair member.
- **Tobias Renn** — friend group / cohort (c01, c03, c06–c07); potential
  stranded-pair member.
- **Headmistress Auria Coyle** — welcomes the intake, sets the ruins test,
  addresses the crisis (c01, c05, c10).
- **Professor Mirabel Quist** — instructor (c04–c05).
- **Professor Silas Thorn** — instructor (c04).

> Open question for a later pass: which named characters make up the *executed*
> stranded pair (`c11_execution`) and the other stranded pairs who murder
> monarchs / open comms in Act III. Candidates: Gideon, Pip, Tobias. Worth fixing
> before the scenes are written so the beat has real faces.
