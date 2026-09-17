<font size="5">**Administration & Permissions**</font>

Administrative commands, access tiers, and individual permissions for **1b1v Lite**.

---

<font size="4">**Admin Commands**</font>

Commands for plugin administration and maintenance:

* `/1b1v reload` — Reloads configuration files and caches without restarting the server.  
  *Permission:* `1b1v.admin.reload`
* `/1b1v notice` — Manages in-game login notifications, alerts, and asset synchronization.  
  *Permission:* `1b1v.admin.notice`

---

<font size="4">**Access Tiers**</font>

Cumulative permission bundles for quick LuckPerms group setup. Each tier includes all permissions from the tiers above it.

| **Tier Node** | **Description** | **Recommended Group** |
| :--- | :--- | :---: |
| `1b1v.basic` | Access to core GUI, basic shapes, generation commands, and simple patterns. | **Default / Builder** |
| `1b1v.intermediate` | Includes `Basic` + procedural brushes (plump, crystal), lianas, grass pattern, and proximity mask. | **Architect / Pro** |
| `1b1v.admin` | Full access to all features and administrative management commands. | **Server Admin** |

---

<font size="4">**Permissions**</font>

All individual permission nodes available in 1b1v Lite.

| **Permission** | **Description** | **Tier** |
| :--- | :--- | :---: |
| `1b1v.use` | `/1b1v`<br>Access to the main 1b1v GUI menu and base commands. | `Basic` |
| `1b1v.generation.platform` | `//platform`<br>Generates a flat square platform or plane. | `Basic` |
| `1b1v.generation.onion` | `//onion`<br>Generates a droplet or onion procedural shape. | `Basic` |
| `1b1v.region.frame` | `//frame`<br>Generates a wireframe along the edges of the selection. | `Basic` |
| `1b1v.region.polygon` | `//polygon`<br>Fills the selection with a polygonal shape. | `Basic` |
| `1b1v.region.centervertical` | `//centerver`<br>Places a vertical pillar through the center of the selection. | `Basic` |
| `1b1v.pattern.ridgedmulti` | `#ridgedmulti`<br>Multi-fractal procedural noise pattern modifier. | `Basic` |
| `1b1v.pattern.flowers` | `#flowers`<br>Generates procedural flower palettes. | `Basic` |
| `1b1v.brush.plump` | `/br plump`<br>Procedural brush for thickening and volumizing shapes. | <nobr>`Intermediate`</nobr> |
| `1b1v.brush.crystal` | `/br crystal`<br>Procedural crystal cluster brush. | <nobr>`Intermediate`</nobr> |
| `1b1v.curve.liana` | `//liana`<br>Generates procedural hanging lianas/vines along a curve. | <nobr>`Intermediate`</nobr> |
| `1b1v.pattern.grass` | `#grass`<br>Generates procedural surface vegetation and grass layers. | <nobr>`Intermediate`</nobr> |
| `1b1v.mask.around` | `#around`<br>Proximity mask detecting blocks adjacent to existing geometry. | <nobr>`Intermediate`</nobr> |
| `1b1v.admin.reload` | `/1b1v reload`<br>Allows reloading plugin configurations and caches. | `Admin` |
| `1b1v.admin.notice` | `/1b1v notice`<br>Allows managing update alerts and syncing assets. | `Admin` |