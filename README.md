# Where Did I Put It?

Find where you left something. Search remembered storage, nearby dropped items, backpacks and recent item movements without leaving Valheim.

**Beta 0.1.2. Provided as-is.**

## Getting started

Install on your own PC through your mod manager, or place `WhereDidIPutIt.dll` in `BepInEx/plugins/WhereDidIPutIt/`. Requires BepInExPack Valheim. A server installation is not required.

Join a world and open the chests you want to remember. Close the inventory, then press **Left Ctrl + F9** to search.

- **Last locations** shows matching items in remembered containers, on the ground and in your carried inventories.
- **Observed history** shows transfers and other item changes your client observed.
- **Locate local** closes the menu and pings a nearby remembered chest or dropped item with a pulsing gold ring and floating marker for 12 seconds.
- **View map** opens your map at the selected location, with a highlighted marker for 90 seconds. If the chest or item is loaded nearby, the marker follows its current position; otherwise it shows the last recorded location.
- Press **Escape**, the shortcut, or the close button to return to the game.

The menu uses a Valheim-inspired wood and bronze frame with warm gold text. Search by item, container type, or action. Names follow the game's language where available. Change the shortcut, window scale, local ping duration, history limits and observation distance in `BepInEx/config/VariantMods.WhereDidIPutIt.cfg` or a configuration manager.

## Remembered locations

Every storage result is a last-seen record. Other players, automatic storage, moving boats, world resets and events while you were offline can change what is there. Open a container again to refresh it. A remembered location is not proof of who moved an item.

The mod records containers you open or use through observed transfers. It refreshes known, accessible containers nearby. It does not search unopened storage across the world. History begins when the mod is installed.

Nearby dropped items appear as **Ground** locations. Their recorded position updates as they roll or float. Your successful pickups remove that ground location. Other players, automatic stacking and despawning can leave an old record; last-seen ground locations are not a promise that the item is still there. Ground locations are kept for up to one real day, with a limit of 300.

Your character and each world have separate local histories. These files are kept under `BepInEx/config/WhereDidIPutIt/history`. Keep that folder out of shared profiles and modpack exports. To erase a history, close Valheim and remove its files from that folder.

## Playing with other mods

Where Did I Put It? reads item lists instead of inventory slots or UI layouts. It supports expanded inventories and container sizes, with optional handling for Smoothbrain Backpacks, CurrencyPocket, EpicLoot names and MultiUserChest pending transfers.

With MultiUserChest, observations wait until pending transfers settle. If a future version changes the information needed to check transfers, live tracking pauses and your saved history remains available.

Quick stacking, crafting from storage, recycling and automatic storage may produce general observed-change entries when the exact cause cannot be identified. Custom storage systems that do not expose ordinary inventories may not appear. It does not require Jotunn or any of these optional mods.

Both markers are private to your client and temporary. Locate local requires a nearby, loaded chest or item you can access; its default range is 40 metres. It follows moving cargo and dropped items, and stops when access is lost. Selecting another location replaces the previous marker. View map is unavailable in no-map worlds, while Locate local still works. Use client mods according to your server's rules.

## Removing the mod

Close Valheim and remove the DLL or uninstall it through your mod manager. The mod does not add items or change world and character save formats. You may keep the local history folder for later use.
