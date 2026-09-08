# Andy's Soulbound Inventory 0.1.2

Fixes the XP-release entity error found in the Bedrock Content Log after the 0.1.1 playtest.

- Removes an obsolete entity component that prevented the invisible XP-release helper from loading on the current retail schema.
- Restores recoverable XP-orb release at the death location after Vanilla XP loss is verified.
- Renames native server commands to unique `asi:soulbound_*` names to avoid generic command-alias conflicts with other add-ons.
- Keeps existing world settings, player choices, pack UUIDs, and inventory behavior.

After importing 0.1.2, test one Vanilla XP-loss death and confirm that recoverable orbs appear once and the Content Log has no `xp_release` actor-definition error. The new console commands are `asi:soulbound_help`, `asi:soulbound_status`, `asi:soulbound_set`, and `asi:soulbound_player`.

Automated tests, stable API type-checking, archive validation, Achievement Friendly, and Vibrant Visuals checks passed. Multiplayer and BDS remain unverified because the owner cannot test them locally.
