SafeArmLink v0.4.0 — Source project
Target: Minecraft Java 1.21.1 + NeoForge 21.1.x + Create 6.0.10
Java: 21

FEATURES IMPLEMENTED IN SOURCE
- Link Plate block registered in Creative Mode.
- Place the plate directly on top of an inventory block.
- Right-click with an item to set a single-item whitelist filter (item + components).
- Shift + right-click with an empty hand to clear the filter.
- Right-click with an empty hand to toggle the plate's visual INPUT/OUTPUT mode.
- Registers a Create ArmInteractionPointType so a Mechanical Arm can target the plate.
- The arm point accesses the inventory capability on the block below the plate.
- Filter is applied both to deposits and extraction; extraction is simulated before removing an item.

IMPORTANT LIMITATIONS
- This source project has NOT been compiled or tested in Minecraft in this environment.
- No ready-to-install .jar is included. Do not rename the ZIP or a random file to .jar.
- Create's Mechanical Arm has its own saved DEPOSIT/TAKE point mode. After selecting the plate as an arm target, verify/toggle the point mode in-game so it matches the plate's visual mode. The plate's visual mode itself does not automatically rewrite an already saved arm configuration.
- The inventory must expose NeoForge Capabilities.ItemHandler.BLOCK from its upper face.
- Filter supports one exact item stack type, not a list or item tags.

BUILD
- Requires Java 21 and a Gradle installation compatible with NeoForge ModDevGradle 2.0.107.
- Requires internet access to download NeoForge, Create 6.0.10, and their dependencies.
- Run: gradle build
- Output, if the build succeeds: build/libs/safearmlink-0.4.0.jar

This package is source code, not a tested compiled mod. Build and test before placing any JAR in a CurseForge profile.
