# Lamp
[![](https://jitpack.io/v/Revxrsal/Lamp.svg)](https://jitpack.io/#Revxrsal/Lamp)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
## Background
<details>
  <summary>Click to expand!</summary>
Building commands has always been a core concept in many applications, and, lots of times, a really boring and cumbersome one to pull off: Having to think of all the possible input from the user, all the mistakes they will make, validating input and then finally executing the actual command logic. 

We *aren't* supposed to mess our hands up with so much of this. We really shouldn't get ourselves dirty with the highly error-prone string manipulation, nor are we supposed to repeat 3 lines of code a thousand times. We also should not be forced to think of all the edge cases and possible output of the user side. Developers should focus on what's *important*, not what isn't.

Then after all that, we really should make sure our code is clean, maintainable, extendable and flexible.

Building upon this belief, Lamp was born.

Lamp has taken responsibility upon itself to take all the crap of the command creation process: parsing input, validating arguments, auto completions, tokenizing and redirection, and leaves you only to the important part of your job here: the actual command logic.

Through annotations, parameter resolvers, command conditions, permissions, argument validators, cooldowns, dependency injection, auto-completers, Lamp not only makes the command creation process much easier, it also becomes more fun, intuitive and less error prone.
</details>

## There are many commands frameworks out there, why should I use Lamp?
Glad you asked!
- **Lamp is small in size**: The overall size of Lamp will not exceed 150 KB. Built to be lightweight, Lamp is convenient to package and ship.
- **Lamp is extendable**: Lamp has been built thoroughly with this in mind. You can create custom annotations for commands, parameters, permissions and resolvers, with their very own functionality. This gives so much space for your own extendability, and also helps make sure the code you write is minimal.
- **Lamp is portable**: Created with a high-level command API and an extendable codebase, Lamp has been produced to provide first-class support to as many platforms as possible. As of now, Lamp supports the following platforms:
    - [Bukkit / Spigot](bukkit)
    - [BungeeCord](bungee)
    - [VelocityPowered](velocity)
    - [SpongePowered](sponge)
    - [Java Discord API (JDA)](jda)
    - [Bare-boned command line interface (CLI)](cli)

   With the help of the built-in APIs for dispatching commands and auto-completions, it is possible to support almost any platform out-of-the-box.
- **Lamp is easy**: Despite all the powerful features and extendability, getting started with Lamp couldn't be easier. Simply create a command handler for your appropriate platform, then proceed with creating your command with the main **\@Command** and **\@Subcommand** annotations, and finally registering it with **CommandHandler#register()**.
- **Lamp is powerful**: Lamp allows you to leverage some of the command features which would be otherwise too burdensome to build:
   - **[@Switch parameters](common/src/main/java/revxrsal/commands/annotation/Switch.java)**
   - **[@Flag (named) parameters](common/src/main/java/revxrsal/commands/annotation/Flag.java)**
   - **[Simple dependency injection](common/src/main/java/revxrsal/commands/annotation/Dependency.java)**
   - **[A quote-aware argument parser](common/src/main/java/revxrsal/commands/command/ArgumentStack.java)**
   - **[Context resolver factories](common/src/main/java/revxrsal/commands/process/ContextResolverFactory.java)** and **[value resolver factories](common/src/main/java/revxrsal/commands/process/ValueResolverFactory.java)**
   - **[Simple and powerful auto completions API](common/src/main/java/revxrsal/commands/autocomplete/AutoCompleter.java)**
   - **[Built-in command cooldown handler](common/src/main/java/revxrsal/commands/annotation/Cooldown.java)**

## Documentation
- **Examples**: [Lamp/examples](https://github.com/Revxrsal/Lamp/tree/examples)
- **Overview**: [Lamp/wiki](https://github.com/Revxrsal/Lamp/wiki)
- **Javadocs**: https://revxrsal.github.io/Lamp/
