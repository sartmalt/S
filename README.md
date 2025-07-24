// index.dm - The Great Eggventure Begins!
// Created by Sarah 🐣
// Featuring the one and only: Humpty Alexander Dumpty

#define GAME_NAME "Humpty's Eggventure"
#define GAME_VERSION "1.0"

// Include game files
#include "code/player.dm"
#include "code/world.dm"
#include "code/egg_logic.dm"
#include "code/humpty.dm"

// World setup
world
    name = GAME_NAME
    version = GAME_VERSION
    hub = "sarah.humptys_eggventure"
    hub_password = 1
    view = "10x10"
    turf = /turf/wall

// World start
world/New()
    ..()
    world << "🥚 Welcome to [GAME_NAME]!"
    world << "✨ Featuring: Humpty Alexander Dumpty, the bravest egg of all time."

// Fun little Easter Egg
/mob/humpty
    name = "Humpty Alexander Dumpty"
    icon = 'icons/humpty.dmi'
    desc = "He's not just an egg... he's *the* egg."
