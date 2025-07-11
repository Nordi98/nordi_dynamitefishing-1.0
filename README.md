
Overview
This script enables dynamite fishing in FiveM with QB-Core and ps-dispatch integration. Players can throw dynamite into water to catch fish, with the risk of triggering a police alert.

Features:
Realistic Dynamite Fishing: Throw a pipe bomb into the water and collect stunned fish.
Skill Check System: Uses ox_lib for timing-based challenges.
Automatic Police Alerts: Explosions are reported to the police via ps-dispatch.
Various Fish Types: Different rarities and rewards.
Cooldown System: Prevents spamming and abuse.

Installation:
Copy the dynamite_fishing folder into your resources directory.
Add ensure dynamite_fishing to your server.cfg.
Make sure the following items exist in qb-core/shared/items.lua:

['dynamite'] = { name = 'dynamite', label = 'Dynamite', weight = 600, ... }
['fish_common'] = { name = 'fish_common', label = 'Common Fish', weight = 200, ... }
['fish_uncommon'] = { name = 'fish_uncommon', label = 'Uncommon Fish', weight = 300, ... }
['fish_rare'] = { name = 'fish_rare', label = 'Rare Fish', weight = 500, ... }
Restart your server or reload the resource.

Usage:

Command: /dynamitefish – Starts dynamite fishing (only when facing water).
Item Use: Use the pipe bomb from your inventory.
Skill Check: Pass the timing challenge to trigger the explosion.
Collecting: Fish are automatically collected after the explosion.

Configuration
You can customize the following in config.lua:

Required item and cooldown time
Skill check difficulty
Explosion parameters
Fish rewards and rarities

Dependencies:
QB-Core Framework
ox_lib (for skill checks)
ps-dispatch (for police alerts)

Credits
Developed by Nordi Designes

Discord for Support: https://discord.gg/QpZsNS6CGz
