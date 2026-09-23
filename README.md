# Backroom Ops

A brand-neutral, mobile-first browser dashboard for backroom shifts. It is a single HTML file with no server, account, build step, or external dependencies.

## Use

Download `index.html` and open it in a current browser. Data is saved in that browser's local storage. Use **Settings → Export JSON backup** regularly and before changing devices or clearing browser data.

The pallet board depicts Standard (mixed cartons), 2-Wave (two wave boxes below mixed cartons), and 4-Wave (four wave boxes) pallets. Select a pallet to open its large target timer. The default target is 15 minutes and can be changed in Settings or per pallet. Actual cartons and wave-box pieces are entered separately. Optional contents samples describe a pallet's actual merchandise without changing its counted cartons or pieces.

New staff start Off shift. Tap Work on each person to begin counting labor time; marking the shift start does not start staff timers. Labor assignments include Unloading / Sorting, Hanging, Layup, Processing, Pushing Freight, Setup / Cleanup, and Miscellaneous. Breaks, lunch, and Off shift are excluded. Hanging and Layup are reported separately and together as clothing work. Beginning and remaining totes accept stacks plus loose totes; four totes make a stack.

The truck timeline records arrival, first box on the belt, and belt clear. Truck duration begins with the first box and ends when the belt is clear; arrival-to-start is reported separately. Reports show truck man-hours, average truck crew, and overall backroom man-hours.

Pallet Contents uses configurable, color-coded department buttons. Each tap records one regular carton against the selected pallet and updates its carton total. Department names, colors, order, and active status can be changed in Settings without altering historical records.

At end of day, complete the prompts and save the shift. The visual report shows labor allocation, pallet mix, and hanging output. History compares up to 14 recent shifts by actual cartons per unloading/sorting man-hour when both counts and hours are present. A saved shift can be viewed later. New Shift clears current activity but retains history and saved crew.

## Data notes

- Pallet contents samples are separate from actual pallet counts. Counted cartons and wave-box pieces are never added into a single rate.
- Ending hanging stock is required to calculate processed totes and racks. The report leaves unknown values blank rather than presenting them as zero.
- If you need to correct calculated labor time, use the optional override for that work area in End of Day.
- A JSON import validates its structure and asks before replacing current shift, history, and preferences. Export a backup before importing when you want to preserve current data.
- Existing `backroomOpsTabletPro_v2` shift data is migrated when the new page is first opened in the same browser. Old staff assignments do not contain historical time segments; check labor totals for an in-progress migrated shift.

## License

GNU General Public License v3.0; see `LICENSE`. Commercial licensing terms are in `LICENSE-COMMERCIAL.md`.

Created by Danny Morgan / LAB-137.
