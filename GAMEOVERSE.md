# Gameoverse notes

Pufferfish's Attributes (`github.com/pufmat/attributesmod`, LGPL-3.0), branch `26.1` at `c8b65e1` (upstream's
unreleased 0.8.3), built unmodified: `./gradlew :Fabric:build` -> `Fabric/build/libs/puffish_attributes-0.8.3-26.1-fabric.jar`.
Branch `gameoverse-26.1`; `origin` push disabled.

Why not the Modrinth 0.8.2 jar: it crashes when damage reflection or life steal kills the attacker (fixed in
`2c5494f`), and has no `mace_damage` translation. Drop this build for the stock jar once upstream releases 0.8.3+ for
26.1.2 (it's in `scripts/upstream_watch.json`).

Installed for the Skill Forest (`docs/skill-forest-design.md`). Its attributes that duplicate Apothic/vanilla/Artifacts
ones are redirected by `gameoverse-attribute-bridge`; the rest are used as themselves. Both sides (registry sync and
client-predicted mining/movement). `stamina` and `natural_regeneration` do nothing here (Hearty Meals replaces vanilla
hunger healing).
