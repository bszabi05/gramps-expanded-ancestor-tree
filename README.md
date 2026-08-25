# Expanded Ancestor Tree for Gramps

The **Expanded Ancestor Tree** is a custom graphical report plugin for the Gramps genealogy program. It is a heavily enhanced fork of the built-in Ancestor Tree report, completely redesigned to visualize collateral family lines without visual clutter.

## ✨ Features

* **Siblings & Cousins:** Displays not only direct ancestors but also their siblings, spouses, cousins, and collateral descendants through recursive family branches.
* **Smart Connection Routing:** Replaces the standard intersecting lines with a custom "circuit-board" style routing system. Collateral family lines are offset from the main ancestral trunk.
* **Bridged Intersections:** When a collateral line crosses the main ancestral line, a small semi-circular "bridge" (jump) is drawn, making the tree much easier to read.
* **Color-Coded Families:** An optional setting to generate distinctly colored connection lines for each separate family group.
* **Modern Typography & Design:** Heavy drop shadows have been removed for a cleaner "flat" design, and personal names are dynamically rendered in **bold** to stand out from dates and places.
* **Auto-Compression:** The graph layout engine automatically compresses vertical space,

## 📥 Installation

1. Download the `ExpandedAncestorTree.zip` release.
2. Extract the folder into your Gramps user plugins directory:
   * **Windows:** `%APPDATA%\gramps\gramps60\plugins\`
   * **Linux:** `~/.gramps/gramps60/plugins/`
   * **macOS:** `~/Library/Application Support/gramps/gramps60/plugins/`
3. Restart Gramps.
4. Go to **Reports -> Graphical Reports -> Expanded Ancestor Tree**.

## ⚙️ Configuration

In the report dialog, you will find new options under the **Tree Options** and **Display** tabs:
* Check *Include siblings of the center person*
* Check *Include siblings of ancestors*
* Check *Include cousins and collateral relatives*
* Check *Use random colors for family lines* (Found under the Display tab).

## 📜 License & Credits

This plugin is released under the **GNU General Public License (GPL) v2 or later**.

* **Original Ancestor Tree Code:** Donald N. Allingham, Brian G. Matherly, Jakim Friant, Paul Franklin, Craig J. Anderson.
* **Expanded Logic & Smart Routing (2026):** Bartok Szabolcs (kotrabdev)
