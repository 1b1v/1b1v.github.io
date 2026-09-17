# Administration & Permissions

Comprehensive guide to administrative commands and permission nodes for **1b1v Lite**.

---

## 🛠 Admin Commands

Administrative commands for configuring and maintaining the plugin in-game.

### `/1b1v reload`
Reloads plugin configuration files, language assets, and internal caches without restarting the server.
* **Permission:** `1b1v.admin.reload`

### `/1b1v notice`
Manages in-game update notices, critical alerts, and preset synchronization.
* **Permission:** `1b1v.admin.notice`

---

## 🛡 Access Tiers (Quick Setup)

Instead of assigning dozens of individual nodes, you can grant pre-configured cumulative tiers to your LuckPerms groups. Each tier automatically includes all permissions from the previous one.

| Tier Node | Recommended Group | Description |
| :--- | :--- | :--- |
| `1b1v.basic` | **Default / Builder** | Essential generation commands, shapes, and basic flora patterns. |
| `1b1v.intermediate` | **Architect / Pro** | Includes `Basic` + advanced brushes, masks, and curved generation. |
| `1b1v.admin` | **Server Admin / Operator** | Full access to all features and administrative commands. |

> ℹ️ **Note:** The tiers are cumulative. Granting `1b1v.intermediate` automatically inherits `1b1v.basic`.

---

## 📋 Permission Nodes

### Core & Administration
| Permission | Command / Feature | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.use` | `/1b1v` | `Basic` | Access to the main 1b1v GUI menu and base commands. |
| `1b1v.admin.reload` | `/1b1v reload` | `Admin` | Access to reload configuration and caches. |
| `1b1v.admin.notice` | `/1b1v notice` | `Admin` | Allows receiving update alerts and maintenance notifications. |

### Selection & Generation
| Permission | Command | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.selection.posboth` | `//pos12` | `Basic` | Sets both selection points simultaneously. |
| `1b1v.selection.outsetnear` | `//osn` | `Basic` | Creates a cuboid selection around the player with a custom radius. |
| `1b1v.generation.platform` | `//platform` | `Basic` | Generates a flat platform or square plane. |
| `1b1v.generation.onion` | `//onion` | `Basic` | Generates an onion/droplet procedural shape. |

### Region Modification
| Permission | Command | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.region.frame` | `//frame` | `Basic` | Generates an outer wireframe along selection edges. |
| `1b1v.region.polygon` | `//polygon` | `Basic` | Fills the selection with a polygonal prism shape. |
| `1b1v.region.centervertical` | `//centerver` | `Basic` | Places a vertical pillar through the center of the selection. |

### Curves
| Permission | Command | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.curve.liana` | `//liana` | `Intermediate` | Generates procedural hanging vines and lianas along a curve. |

### Brushes
| Permission | Command | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.brush.crystal` | `/br crystal` | `Intermediate` | Procedural crystal cluster brush. |
| `1b1v.brush.plump` | `/br plump` | `Intermediate` | Procedural shape volumizer/thickening brush. *(if enabled in Lite)* |

### Custom Patterns & Masks
| Permission | Syntax | Tier | Description |
| :--- | :--- | :---: | :--- |
| `1b1v.pattern.ridgedmulti` | `#ridgedmulti` | `Basic` | Ridged-multifractal procedural noise pattern. |
| `1b1v.pattern.flowers` | `#flowers` | `Basic` | Generates procedural flower palettes. |
| `1b1v.pattern.grass` | `#grass` | `Intermediate` | Generates procedural surface vegetation and grass layers. |
| `1b1v.mask.around` | `#around` | `Intermediate` | Proximity mask detecting blocks adjacent to existing geometry. |