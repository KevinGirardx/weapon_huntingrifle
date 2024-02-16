###### HUNTING RIFLE TO BE USED WITH #########
https://kevin-scripts.tebex.io/package/5232160
https://kevin-scripts.tebex.io/package/5232160
https://kevin-scripts.tebex.io/package/5232160


# Add the following in qb-core > shared > items.lua
```lua
    weapon_huntingrifle          = { name = 'weapon_huntingrifle',          label = 'Hunting Rifle',                            weight = 1000, type = 'weapon',         ammotype = 'AMMO_SNIPER',               image = 'weapon_huntingrifle.png',          unique = true,      useable = true,     description = 'Weapon for hunting Big or Small Game.' },

```

# Next add the following in qb-core > shared > weapons.lua
```lua
    [`weapon_huntingrifle`]          = { name = 'weapon_huntingrifle', label = 'Hunting Rifle', weapontype = 'Sniper Rifle', ammotype = 'AMMO_SNIPER', damagereason = 'Sniped / Picked off / Scoped' },
```

# IF you're using ox_inventory add the following in the weapon.lua

```lua
    ['WEAPON_HUNTINGRIFLE'] = {
        label = 'Hunting Rifle',
        weight = 10000,
        durability = 0.5,
        ammoname = 'ammo-sniper'
    },
```

# Add the following in qb-smallresources > client > weapdraw.lua withing the local weapons table

```lua
    'WEAPON_HUNTINGRIFLE',
```

# Add the following in qb-smallresources > client > recoil.lua

```lua
    [`weapon_huntingrifle`] = 0.2,
```

# Add the following in ps-dispatch > client > cl_events.lua
```lua
    [`weapon_huntingrifle`] = "CLASS 3: Hunting Rifle",
```

Credits:
https://www.gta5-mods.com/weapons/sauer-101-hunting-rifle-animated-4k