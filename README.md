MidnightNameplates

MidnightNameplates is a modern, highly customizable nameplate addon for World of Warcraft: Midnight, built as part of the Midnight addon series.

It is designed around three goals:

Clarity • Customization • Performance

MidnightNameplates provides the tools expected from a full nameplate replacement while maintaining its own original architecture, configuration interface, visual identity, and gameplay systems.

Features
Nameplate Support

Separate handling and customization for:

Enemy NPCs
Enemy players
Friendly players
Friendly pets and minions
Enemy pets and minions
Guardians
Totems
Elite and other unit classifications

Summoned-unit visibility depends on the nameplate sources Blizzard exposes to addons.

Health Bars

Customize nameplate health presentation with controls for:

Width
Height
Scale
Alpha
Health colors
Textures
Borders and presentation
Unit-type-specific appearance
Normal and Thin summon styles

SharedMedia resources are supported where applicable.

Names & Typography

Customize unit-name presentation independently from the health bar.

Options include:

Font
Font size
Name color
Positioning
Unit-type-specific presentation
SharedMedia fonts
Target, Focus & Mouseover

MidnightNameplates provides dedicated visual emphasis for:

Current target
Focus
Mouseover
Non-target units
Target indicators

This allows important units to stand out without requiring every visible nameplate to be oversized.

Cast Bars

Integrated cast bars provide important spell information directly on the nameplate.

Features include:

Spell name
Spell icon
Cast timer
Interruptible state
Non-interruptible state
Channel support
Configurable appearance and positioning

The cast system is designed around the restrictions of the modern WoW API, including protected and secret values.

Auras

Display combat-relevant buffs and debuffs directly around nameplates.

Supported information includes:

Buffs
Debuffs
Durations
Stack counts
Multiple aura presentation
Configurable aura behavior
Threat & Combat Awareness

MidnightNameplates includes combat-oriented visual systems for:

Threat
Combat state
Classification indicators
Priority indicators
Execute presentation
Unit-specific emphasis

These systems are especially useful when dealing with large groups of enemies in dungeons and Mythic+.

PvE Intelligence & Rules

The Rules and Intelligence systems provide additional control over how important units are presented.

They are designed to complement the normal nameplate configuration rather than force the player into a predefined layout.

Build anything from a minimal open-world setup to a more information-heavy dungeon, raid, or Mythic+ profile.

Pets, Minions, Guardians & Totems

Summoned units have dedicated configuration rather than simply inheriting every normal NPC setting.

Available controls include:

Friendly Pet / Minion
Enemy Pet / Minion
Guardian
Totem
Enable / disable
Health
Names
Cast bars where applicable
Auras where applicable
Width and height
Scale
Alpha
Normal / Thin styles
Blizzard summon sources

World of Warcraft controls whether some summoned-unit nameplate sources are exposed to addons.

MidnightNameplates deliberately avoids continuously modifying or fighting Blizzard's source CVars.

If a pet or minion is not exposed, check:

WoW → Options → Nameplates → Minions

Once Blizzard exposes a supported plate, MidnightNameplates can style it.

Profiles

MidnightNameplates includes a complete profile system.

Profiles support:

Create
Copy
Rename
Delete
Default-profile protection
Per-character profiles
Automatic context profiles
Import
Export

Imports include preview, validation, and confirmation before replacing configuration data.

Live Preview

The configuration interface contains an integrated live preview.

Preview supported nameplate families and states while adjusting settings without needing to find the appropriate unit in the game world.

This includes different unit types and targeting states.

Configuration

MidnightNameplates uses its own Midnight-style configuration interface.

Major sections include:

Info
General
Health
Name
Target
Indicators
Cast Bar
Auras
Threat
Unit Types
Summons
Classifications
Rules
Intelligence
Profiles

Configuration pages use dynamic content-aware scrolling rather than forcing every page to share the same scroll range.

MidnightNameplates is also registered with Blizzard's addon settings:

Esc → Options → AddOns → MidnightNameplates

Performance

Nameplates can become expensive when large numbers of units are visible.

MidnightNameplates development therefore includes dedicated performance work focused on:

Dense nameplate environments
Avoiding unnecessary polling
Reducing repeated updates
Coalescing repeated work
Blizzard visual suppression
Duplicate plate prevention
Friendly-player performance
WoW 12.1 protected-action restrictions
WoW 12.1 secret-value restrictions

Development diagnostics are read-only and run only when explicitly requested.

Installation
Download the latest MidnightNameplates release.
Extract the archive.
Place the MidnightNameplates folder inside:
World of Warcraft/_retail_/Interface/AddOns/
Start World of Warcraft or /reload if the game is already running.
Type:
/mnp
Commands
Command	Description
/mnp	Open MidnightNameplates
/midnightnameplates	Open MidnightNameplates
/mnpsummoncheck	Validate summon/nameplate configuration
/mnpsummon	Run detailed summon diagnostics
Diagnostics

MidnightNameplates contains advanced troubleshooting tools intended for development, support, and future WoW API changes.

Available through:

/mnpsummoncheck
/mnpsummon

or:

MidnightNameplates → Info → Advanced Diagnostics

Diagnostics are:

Read-only
On-demand
Not continuously polling
Not intended to modify Blizzard nameplate settings
Compatibility
	
MidnightNameplates	12.0.0
World of Warcraft	Midnight / 12.1
Interface	120100
Author	Arrakeen_EU
Development Philosophy

MidnightNameplates is built around a simple principle:

Provide the depth of a mature nameplate addon without sacrificing stability, performance, or control.

The addon has gone through dedicated development phases covering:

Core nameplate architecture
Unit classification
Cast bars
Auras
Threat
Targeting
Summoned units
PvE intelligence
Profiles
Import/export
Live preview
Performance optimization
Blizzard coexistence
WoW 12.1 compatibility
Real-gameplay validation

The stable 12.0.0 release was promoted from a feature-frozen RC baseline.

Midnight Addon Series

MidnightNameplates is part of the Midnight addon family.

Each Midnight addon is designed to work independently while sharing a consistent design philosophy and visual language.

Contributing & Bug Reports

When reporting a problem, please include:

MidnightNameplates version
WoW version
What type of content you were playing
Steps to reproduce the issue
Any Lua error
Whether other nameplate addons were enabled

For pet/minion issues, also include the output from:

/mnpsummoncheck

For more detailed troubleshooting:

/mnpsummon
Copyright & Originality

Copyright © 2026 Arrakeen_EU.

MidnightNameplates is an independently developed project with its own codebase, configuration system, branding, visual design, and artwork.

It is not intended to contain or redistribute proprietary code, artwork, logos, or other copyrighted assets from third-party nameplate addons.

World of Warcraft, Blizzard Entertainment, and related names and trademarks are property of their respective owners.

MidnightNameplates is an independent community project and is not affiliated with or endorsed by Blizzard Entertainment.
