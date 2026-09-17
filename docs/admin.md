# Administration & Permissions

Administrative commands, access tiers, and individual permissions for **1b1v Lite**.

---

### Admin Commands

Commands for plugin administration and maintenance:

* `/1b1v reload` — Reloads configuration files and caches without restarting the server.  
  *Permission:* `1b1v.admin.reload`
* `/1b1v notice` — Manages in-game login notifications, alerts, and asset synchronization.  
  *Permission:* `1b1v.admin.notice`

---

### Access Tiers

Cumulative permission bundles for quick LuckPerms group setup. Each tier includes all permissions from the tiers above it.

| **Tier Node** | **Description** | **Recommended Group** |
| :--- | :--- | :---: |
| `1b1v.basic` | Access to core GUI, basic shapes, generation commands, and simple patterns. | **Default / Builder** |
| `1b1v.intermediate` | Includes `Basic` + procedural brushes (plump, crystal), lianas, grass pattern, and proximity mask. | **Architect / Pro** |
| `1b1v.admin` | Full access to all features and administrative management commands. | **Server Admin** |

---

### Permissions

All individual permission nodes available in 1b1v Lite.

| **Permission** | **Description** | **Tier** |
| :--- | :--- | :---: |
| `1b1v.use` | `/1b1v` — Access to the main 1b1v GUI menu and base commands. | `Basic` |
| `1b1v.generation.platform` | `//platform` — Generates a flat square platform or plane. | `Basic` |
| `1b1v.generation.onion` | `//onion` — Generates a droplet or onion procedural shape. | `Basic` |
| `1b1v.region.frame` | `//frame` — Generates a wireframe along the edges of the selection. | `Basic` |
| `1b1v.region.polygon` | `//polygon` | `Basic` |
| `1b1v.region.centervertical` | `//centerver` — Places a vertical pillar through the center of the selection. | `Basic` |
| `1b1v.pattern.ridgedmulti` | `#ridgedmulti` — Multi-fractal procedural noise pattern modifier. | `Basic` |
| `1b1v.pattern.flowers` | `#flowers` — Generates procedural flower palettes. | `Basic` |
| `1b1v.brush.plump` | `/br plump` — Procedural brush for thickening and volumizing shapes. | `Intermediate` |
| `1b1v.brush.crystal` | `/br crystal` — Procedural crystal cluster brush. | `Intermediate` |
| `1b1v.curve.liana` | `//liana` — Generates procedural hanging lianas/vines along a curve. | `Intermediate` |
| `1b1v.pattern.grass` | `#grass` — Generates procedural surface vegetation and grass layers. | `Intermediate` |
| `1b1v.mask.around` | `#around` — Proximity mask detecting blocks adjacent to existing geometry. | `Intermediate` |
| `1b1v.admin.reload` | `/1b1v reload` — Allows reloading plugin configurations and caches. | `Admin` |
| `1b1v.admin.notice` | `/1b1v notice` — Allows managing update alerts and syncing assets. | `Admin` |