# warframe-kim-dialogues

All Kinemantik Instant Messaging conversations and various ways to explore them.

- [Kimulacrum](https://kim.browse.wf/kimulacrum.html) — web-based reimplementation of the KIM chat allowing you to take all conversations and paths. This fork allows the user play through of KIM chats as if in-game. （Does not currently hand state variables across Hex members.)
- [Minesweeper](https://kim.browse.wf/minesweeper.html) — Generates segments of chat conversations with the Drifter response that will result in failed romance with the selected Hex member.
- [Convo Locator](https://kim.browse.wf/convo-locator.html) — find a conversation based on (part of) a message
- [Flowcharts](flowcharts)

## Stockfish

The stockfish script will look through your chatlogs to tell you which choices were suboptimal. To use it:

1. Ensure you have [Pluto](https://pluto-lang.org/docs/Getting%20Started) installed
2. Get your inventory either [via AlecaFrame](https://sainan.github.io/alecaframe-inventory-parser/) or [directly](https://github.com/Sainan/warframe-api-helper) and put it in inventory.json
3. Run `pluto stockfish.pluto`

## Scripts

- extract.bat: Invokes [Warframe Exporter](https://github.com/Puxtril/Warframe-Exporter) to extract the raw `*Dialogue_rom.dialogue` files. Makes some assumptions specific to my environment.
- Hell-Scrubber: Parses the raw `*Dialogue_rom.dialogue` files into the JSON files you can see here. Makes some assumptions specific to my environment.
- Dotinator: Converts the JSON files into DOT format then invokes Graphviz to make the flowchart PNGs.
