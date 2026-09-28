# Easier Hydrogen

NeoForge 1.21.1 addon for Mekanism. Adds simple **Chemical Oxidizer** recipes
(one item in, one chemical out) so common chemicals are easy to make.

| Chemical | Input (1 item) | Output |
|---|---|---|
| Hydrogen | Snowball | 100 mB |
| Hydrogen | Ice | 400 mB |
| Hydrogen | Snow block | 400 mB |
| Hydrogen | Packed ice | 800 mB |
| Hydrogen | Blue ice | 1600 mB |
| Hydrogen | Water bucket | 1000 mB |
| Oxygen | Any leaves (`#minecraft:leaves`) | 100 mB |
| Chlorine | White dye | 100 mB |
| Sodium | Dried kelp | 100 mB |
| Ethene | Apple | 100 mB |
| Ethene | Sugar cane | 100 mB |
| Sulfur dioxide | Gunpowder | 50 mB |
| Hydrofluoric acid | Fluorite (`#c:gems/fluorite`) | 100 mB |
| Helium | Glowstone dust | 100 mB (only if Mekanism: Sun is installed) |

## Alloyer (Mekanism: Sun)
| Inputs | Output |
|---|---|
| 1 Electrum ingot + 1 Lapis lazuli + 100 mB helium | 2 Raw uranium |
| 1 Gold ingot + 1 Iron ingot + 100 mB helium | 2 Electrum ingots (replaces the silver recipe) |

## Build on GitHub
1. Push the **contents** of this folder (so `build.gradle` is at the repo root) to a GitHub repo.
2. Open the **Actions** tab. The `Build` workflow runs on every push.
3. Download the jar from the run's **Artifacts** section (`easier-hydrogen`).
4. Drop it in your `mods` folder next to Mekanism 10.7.x.

## Build locally
Needs JDK 21 and Gradle 8.10+: `gradle build` -> `build/libs/`.

## Tweak or add recipes
Recipes live in `src/main/resources/data/mekanism/recipe/oxidizing/<chemical>/`.
Copy any file, change the `input` item/tag and the `output` id/amount.
