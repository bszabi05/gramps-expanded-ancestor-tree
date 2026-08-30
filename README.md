# Expanded Ancestor Tree for Gramps

The **Expanded Ancestor Tree** is a custom graphical report plugin for the Gramps genealogy program. It is a heavily enhanced fork of the built-in Ancestor Tree report, completely redesigned to visualize collateral family lines without visual clutter.

## Features

* **Expanded View:** Shows direct ancestors along with their siblings.
* **Cousin Support:** Optionally display the descendants of the ancestors' siblings.
* **Center Person Descendants:** Optionally display the spouse(s) and full descending lines (children, grandchildren) of the center person.
* **Smart Routing:** Intelligently draws intersecting family branches with clean, bridged lines to prevent visual confusion.
* **Dynamic Colors:** Option to draw each family's connecting lines with a distinct color.
* **Modern Design:** Clean, flat box design with bold typography for easier readability.
* **Safety Limits:** Built-in failsafe prevents memory issues by aborting the generation if t

* **Siblings & Cousins:** Displays not only direct ancestors but also their siblings, spouses, and cousins.
* **Smart Connection Routing:** Replaces the standard intersecting lines with a custom "circuit-board" style routing system. Collateral family lines are offset from the main ancestral trunk.
* **Bridged Intersections:** When a collateral line crosses the main ancestral line, a small semi-circular "bridge" (jump) is drawn, making the tree much easier to read.
* **Color-Coded Families:** An optional setting to generate distinctly colored connection lines for each separate family group.
* **Modern Typography & Design:** Heavy drop shadows have been removed for a cleaner "flat" design, and personal names are dynamically rendered in **bold** to stand out from dates and places.
* **Auto-Compression:** The graph layout engine automatically compresses vertical space, eliminating the huge gaps seen in standard reports when ancestors are unknown.

### v1.0.3
* **Fix:** Smart-routing connection lines now render correctly across multiple page when "Scale tree to fit" is disabled
* **Fix:** Fixed and optimized PDF and SVG generation for multi-page layouts.


### v1.0.2

* **Enhancement:** Added a `Descendant Generations` limit to the UI (Tree Options) to control how deep the downward branches grow.
* **Fix:** Replaced the hard crash on large trees with a graceful soft limit. The engine now safely halts expansion at 250 people, displays a warning dialog, and successfully generates the report with the discovered individuals without freezing Gramps.

### v1.0.1

* **Feature:** Added support for showing the center person's spouse and full descending lines (toggleable in Tree Options).
* **Fix:** Implemented a smart routing algorithm for connecting lines. Bridges are now only drawn at actual physical intersections.
* **Fix:** Corrected horizontal cascade geometry so family branch lines perfectly align with sibling/cousin offsets.
* **Enhancement:** Added limits to prevent performance issues and freezing on massive family trees.
* **UI:** Renamed the report display name to "Ancestor Tree Expanded" so it appears adjace

## 📥 Installation

1. Download the latest release package.
2. Extract the folder into your Gramps user plugins directory:
   * **Windows:** `%APPDATA%\gramps\gramps60\plugins\`
   * **Linux:** `~/.gramps/gramps60/plugins/`
   * **macOS:** `~/Library/Application Support/gramps/gramps60/plugins/`
3. Restart Gramps.
4. Go to **Reports -> Graphical Reports -> Expanded Ancestor Tree**.

## ⚙️ Configuration

In the report dialog, you will find new options under the **Tree Options** and **Display** tabs:

* Check *Include descendants of the center person*
* Check *Include siblings of the center person*
* Check *Include siblings of ancestors*
* Check *Include cousins*
* Check *Use random colors for family lines* (Found under the Display tab).

## 📜 License & Credits

This plugin is released under the **GNU General Public License (GPL) v3**.

* **Original Ancestor Tree Code:** Donald N. Allingham, Brian G. Matherly, Jakim Friant, Paul Franklin, Craig J. Anderson.
* **Expanded Logic & Smart Routing (2026):** Bartok Szabolcs (kotrabdev)
