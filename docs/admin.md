# Administration & Permissions

Administrative commands and permission nodes for **1b1v Lite**.

---

## Admin Commands

Commands for server administration and plugin management:

* `/1b1v reload` — Reloads configuration files and caches without restarting the server.  
  *Permission:* `1b1v.admin.reload`
* `/1b1v notice` — Manages in-game login notifications, critical alerts, and preset synchronization.  
  *Permission:* `1b1v.admin.notice`

---

## Access Tiers

Cumulative permission bundles for quick LuckPerms configuration. Each tier automatically includes all permissions from preceding tiers.

| Tier Node | Recommended Group | Description |
| :--- | :--- | :--- |
| `1b1v.basic` | **Default / Builder** | Core GUI access, basic generation tools, frame/polygon shapes, and simple patterns. |
| `1b1v.intermediate` | **Architect / Pro** | Includes `Basic` + procedural brushes (plump, crystal), lianas, grass pattern, and proximity mask. |
| `1b1v.admin` | **Server Admin** | Grants full access to all features and administrative commands. |

---

## Permissions

All individual permission nodes available in 1b1v Lite.

| Permission | Command / Syntax | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.use` | `/1b1v` | `Basic` | Access to the main 1b1v GUI menu and base commands. |
| `1b1v.generation.platform` | `//platform` | `Basic` | Generates a flat square platform or plane. |
| `1b1v.generation.onion` | `//onion` | `Basic` | Generates a droplet/onion procedural shape. |
| `1b1v.region.frame` | `//frame` | `Basic` | Generates a wireframe along the edges of the selection. |
| `1b1v.region.polygon` | `//polygon` | `Basic` | Fills the selection with a polygonal shape. |
| `1b1v.region.centervertical` | `//centerver` | `Basic` | Places a vertical pillar through the center of the selection. |
| `1b1v.pattern.ridgedmulti` | `#ridgedmulti` | `Basic` | Multi-fractal procedural noise pattern modifier. |
| `1b1v.pattern.flowers` | `#flowers` | `Basic` | Procedural flower generation pattern. |
| `1b1v.brush.plump` | `/br plump` | `Intermediate` | Procedural brush for thickening and volumizing shapes. |
| `1b1v.brush.crystal` | `/br crystal` | `Intermediate` | Procedural crystal cluster brush. |
| `1b1v.curve.liana` | `//liana` | `Intermediate` | Generates hanging lianas/vines along a curve. |
| `1b1v.pattern.grass` | `#grass` | `Intermediate` | Procedural surface vegetation pattern. |
| `1b1v.mask.around` | `#around` | `Intermediate` | Proximity mask detecting blocks adjacent to existing surfaces. |
| `1b1v.admin.reload` | `/1b1v reload` | `Admin` | Allows reloading plugin configurations and caches. |
| `1b1v.admin.notice` | `/1b1v notice` | `Admin` | Allows viewing update alerts and syncing assets. |