# Project context

Durable guidance for the authoring agent.

- The four love interests are Ember Kellan, Isolde Vorn, Seraphine Halcyon, and Wren Ashfield; the protagonist is Caedon Vale. The other characters (Gideon Marsh, Pip Calloway, Tobias Renn, professors Quist/Thorn/Silas, Headmistress Auria Coyle) are not routes. The story has five routes: one per love interest plus a fifth dark polygamy arc that branches when a stranded pair dies.
- The four love interests are Wren Ashfield, Isolde Vorn, Seraphine Halcyon, and Ember Kellan. The protagonist is Caedon Vale. Story is a Cog-College magic academy setting with 'weaves'/channeling, Governors/licensing, and Rust-scarring from ungoverned power.
- The story has five routes: one per love interest (Wren Ashfield, Isolde Vorn, Seraphine Halcyon, Ember Kellan) plus a dark polygamy arc where Caedon falls for all four. Route outlines live in wiki/outline-<id>.md; the shared act skeleton is wiki/outline.md (untouched template).
- Scene format: scenes/ chunks are single-scene Fountain. The working branch markers are
  [[choice:]], [[next:]], [[scene:]] only. The [[line: Ln]] / [[nextline: N]] markers are the
  editor's stable line-id system — edit_scene addresses lines by those ids; leave them in place,
  they are not route logic. There is NO line-level conditional, no per-route line selection, and no
  branch state: a reconvergence forgets which choice was taken. Divergence is scene-level only.
- Academy affinity arc (c06–c11): the old "(Ember path)/(Isolde path)/…" parenthetical "route
  coloring" on the pre-branch spine was inert — every variant rendered on every playthrough. It is
  now real structure: c06_the_ruins ends in a five-way affinity choice into per-affinity chunks
  c07_{em,is,se,wr,ud} → c08_{…} → c09_{…}, all reconverging at c10_the_world_breaks.
  c11b_on_the_run and c11_execution were folded back to shared beats. The definitive route +
  Undivided choice still happens at c11_execution; because there is no state, the early affinity is
  cosmetic foreshadowing and does not constrain the c11 choice.
- Worldbuilding vocabulary (from character sheets): channeling magic is 'the Weave/weaves'; strategic-class weaves act like nukes. Two power-types recur — 'Vash-strong' (raw, ungoverned; e.g. Ember, Wren) and 'Sela-strong' (precise, subtle; e.g. Isolde, Seraphine). 'Rust-scarring' is the bodily cost of ungoverned channeling. Factions/places: the Cog-Colleges/Cograuncy, Assayers & the Grey Hands (who 'sever' channelers), Governors/Ferran licensing, Loomwrights, Kiln-Sworn of the Vashan Dominion, the Grey Principality of Vorn, Halcyon Reach.
- Visual style: the whole VN renders in a Japanese-anime art style. This is set project-wide via `art_style` in project.yaml and applies to every character and location; keep new character/location work consistent with it.
