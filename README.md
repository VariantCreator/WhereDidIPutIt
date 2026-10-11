# 🔎 Where Did I Put It?
### Find the chest. Follow the trail.

Search remembered storage, nearby dropped items, backpacks and recent item movements without leaving Valheim.

**Version 0.1.2 · Client-only · No server installation needed**

## 📦 Install

Requires **BepInExPack Valheim**.

Install on your own PC through your mod manager, or place `WhereDidIPutIt.dll` in `BepInEx/plugins/WhereDidIPutIt/`.

[📥 Downloads](https://github.com/VariantCreator/WhereDidIPutIt/releases)

## 🚀 Get started

1. Join a world and **open the chests you want to remember**.
2. Close the inventory and press **Left Ctrl + F9**.
3. Search by **item, container type or action**.

Names follow the game's language where available. Press **Escape**, the shortcut or the close button to return to the game.

## 🗂️ Find your last locations

- **Last locations** — Matching items in remembered containers, on the ground and in your carried inventories.
- **Observed history** — Transfers and other item changes your client observed.
- **Locate local** — Closes the menu and marks a nearby remembered chest or dropped item with a pulsing gold ring and floating marker.
- **View map** — Opens the map at the selected location with a highlighted marker.

The menu uses a wood and bronze frame with warm gold text.

## 📍 Follow the marker

**Locate local** lasts **12 seconds** by default and works within **40 metres**. The chest or item must be loaded nearby and accessible. The marker follows moving cargo and dropped items, and stops if access is lost.

**View map** highlights a location for **90 seconds**. It follows the current position when the chest or item is loaded nearby; otherwise it shows the last recorded location.

**Both markers are private and temporary.** Selecting another location replaces the previous marker. View map is unavailable in no-map worlds, but Locate local still works.

## 🕒 Remembered, not guaranteed

Storage results are **last-seen records**. Other players, automatic storage, moving boats, world resets and changes while you were offline can leave them out of date. Open a container again to refresh it.

The mod remembers containers you open or use through observed transfers, and refreshes known, accessible containers nearby. **It does not search unopened storage across the world.** History begins when you install the mod.

A remembered location is **not proof of who moved an item**.

### Dropped items

Nearby dropped items appear as **Ground** locations. Their positions update as they roll or float, and your successful pickups remove their ground records.

Other players, automatic stacking and despawning can leave old records. A recorded item may no longer be there. Ground records are kept for **up to one real day**, with a limit of **300**.

## 🎨 Settings & personal history

Change the shortcut, window scale, local ping duration, history limits and observation distance through a configuration manager or:

`BepInEx/config/VariantMods.WhereDidIPutIt.cfg`

Each character and world has its own local history, stored in:

`BepInEx/config/WhereDidIPutIt/history`

**Keep this history folder out of shared profiles and modpack exports.** To erase a history, close Valheim and remove its files from that folder.

## 🧩 Playing with other mods

Supports expanded inventories and container sizes by reading item lists rather than inventory slots or UI layouts.

Optional handling includes **Smoothbrain Backpacks**, **CurrencyPocket**, **EpicLoot names** and **MultiUserChest pending transfers**. Neither Jotunn nor these optional mods is required.

With MultiUserChest, observations wait for pending transfers to settle. If a future version changes the information needed to check them, live tracking pauses and your saved history remains available.

Quick stacking, crafting from storage, recycling and automatic storage may appear as general observed changes when their exact cause cannot be identified. Custom storage that does not expose ordinary inventories may not appear.

Use client mods according to your server's rules.

## 🔄 Removing the mod

Close Valheim and remove the DLL, or uninstall through your mod manager.

The mod does not add items or change world and character save formats. You can keep your local history folder for later use.
