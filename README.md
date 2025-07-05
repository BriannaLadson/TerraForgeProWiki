# TerraForgePro 🗺️
**Procedural Biome/Island & Dungeon Map Generator using Simplex Noise**

**TerraForgePro** is a versatile Python toolset for procedural map generation. 

It includes tools for creating noise-based biome maps and multi-level dungeon layouts with fine-grained control over terrain shaping, biome placement, and dungeon structure.

---
## ⚠️ Important Note!!!
This repo only contains the **Wiki documentation** for [TerraForgePro](https://gum.co/u/rwq2bbml), a **paid** Python map generation library.

- 🧭 **No source code is included** in this repository.
- 🛒 You can [purchase TerraForgePro here on Gumroad](https://gum.co/u/rwq2bbml).
- 🌱 Looking for the **free version**? Check out [TerraForge on GitHub](https://github.com/BriannaLadson/TerraForge).

---

## 🚀 Features
### 🌍 Biome Generator (TerraForgePro)
- Elevation, Moisture, and Temperature map generation
- Supports single and clustered multi-island generation
- Falloff support: Radial, Edge, or None
- Parameters for island spread, spacing, scale, and strength
- Basic biome color mapping based on environmental conditions
- Outputs high-resolution PNG images

## 🏰 Dungeon Generator (DungeonForgePro)
- Multi-level dungeon generation (3D stack of floors)
- Procedural room placement and corridor carving
- Up/down stairs for vertical navigation
- Console-based movement demo included
- Optional PNG export per dungeon level
- Tile color customization for export

---

## 🛠 Requirements

Install the required dependencies:

```bash
pip install numpy noise pillow
```

---

## 🧪 Demos

### Biome Map Generator
Run the included demo script:

```bash
python demo.py
```

The generated maps will be saved as biome_map, elevation_map, moisture_map, temperature_map, (noise_type)_map.

### Dungeon Map Generator
Run either the included dungeon_demo script or dungeon_demo1 script.
```
python dungeon_demo.py
```
Console based demo with movement.

```
python dungeon_demo1.py
```

Generates .pngs for each dungeon level. 

---

## ⚙️ Customization Options

### Biome Generator
Edit the values in terraforgepro.py or the demo to control:

- map_size and image_size

- falloff type: "radial", "edge", or None

- num_islands, island_spread, min_island_spacing

- noise types (elevation, moisture, temperature)

- biome_thresholds for  noise types (elevation, moisture, and temperature)

### Dungeon Generator
- Map size (width, height)
- Number of levels (z_levels)
- Maximum rooms and room size constraints
- Tile symbols and export colors
- Specify which levels to export (levels=[0, 2])

---

## 📁 Included Files
terraforgepro.py – Biome generation engine

dungeonforgepro.py – Dungeon generation engine

demo.py – Biome generation demo

dungeon_demo.py - Dungeon navigation demo

dungeon_demo1.py - Dungeon generation demo

licenses/ – Third-party license files
