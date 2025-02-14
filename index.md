---
layout: home
---

{% assign cacheBust = site.time | date:'?v=%s' %}
![Image]({{ "/images/AstraControlPower-3D_blender_top_angled.png" | absolute_url | append: cacheBust }}){: width="400" }

Power distribution board for input, output, switch, power converter and board screw terminal connectors.
The board connects to [AstraControl](https://liveleds.github.io/AstraControl) ESP32-based control PCB uses WiFi with an external antenna and 5Mbps RS-485.

[![CI](https://github.com/LiveLeds/AstraControlPower/actions/workflows/ci.yml/badge.svg)](https://github.com/LiveLeds/AstraControlPower/actions/workflows/ci.yml)

![GitHub last commit](https://img.shields.io/github/last-commit/liveleds/AstraControlPower?link=https%3A%2F%2Fgithub.com%2FLiveLeds%2FAstraControlPower)

## Table of contents

- [Table of contents](#table-of-contents)
  - [Render Top Angled](#render-top-angled)
  - [Render Top](#render-top)
  - [Render Bottom](#render-bottom)
  - [Schematic](#schematic)
    - [Dark](#dark)
    - [Monochromatic](#monochromatic)
    - [Light](#light)
  - [Assembly](#assembly)
    - [Dark](#dark-1)
    - [Light](#light-1)
    - [Gerber viewer on tracespace.io](#gerber-viewer-on-tracespaceio)
  - [Interactive BOM](#interactive-bom)
  - [BOM](#bom)
  - [Downloads](#downloads)
    - [JLCPCB](#jlcpcb)
    - [Eurocircuits](#eurocircuits)
    - [3D Step](#3d-step)
- [Report](#report)
    - [ERC](#erc)
    - [DRC](#drc)
- [Know Issues](#know-issues)
- [Credits](#credits)

### Render Top Angled

![Image]({{ "/images/AstraControlPower-3D_blender_top_angled.png" | absolute_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/AstraControlPower-3D_blender_top.png" | absolute_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/AstraControlPower-3D_blender_bottom.png" | absolute_url | append: cacheBust }})

### Schematic

#### Dark

- [Schematic Dark PDF]({{ "/documents/AstraControlPower-schematic-dark.pdf" | absolute_url | append: cacheBust }})

#### Monochromatic

- [Schematic Monochromatic PDF]({{ "/documents/AstraControlPower-schematic-mono.pdf" | absolute_url | append: cacheBust }})

#### Light

- [Schematic Light PDF]({{ "/documents/AstraControlPower-schematic-default.pdf" | absolute_url | append: cacheBust }})

### Assembly

#### Dark

- [PCB Dark PDF]({{ "/documents/AstraControlPower-pcb-dark.pdf" | absolute_url | append: cacheBust }})

#### Light

- [PCB Light PDF]({{ "/documents/AstraControlPower-pcb-light.pdf" | absolute_url | append: cacheBust }})

#### Gerber viewer on tracespace.io

[https://tracespace.io/view/?boardUrl={{ "export/AstraControlPower-JLCPCB.zip" | absolute_url | append: cacheBust }}](https://tracespace.io/view/?boardUrl={{ "export/AstraControlPower-JLCPCB.zip" | absolute_url | append: cacheBust }})

### Interactive BOM

Check component locations by hovering over a specific component.
The visual elements might not be precise enough for pcb review but can be very useful since it's possible to pan and zoom.
Not all BOM columns are available here, for datasheet links see BOM below.

[IBOM HTML]({{ "/export/AstraControlPower-ibom.html" | absolute_url | append: cacheBust }})

### BOM

All components with Values, References, Sheetpath and Links to the datasheet.

[BOM HTML]({{ "/export/AstraControlPower-bom.html" | absolute_url | append: cacheBust }})

### Downloads

#### JLCPCB

- [JLCPCB Zip]({{ "export/AstraControlPower-JLCPCB.zip" | absolute_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/AstraControlPower_bom_jlc.csv" | absolute_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/AstraControlPower_cpl_jlc.csv" | absolute_url | append: cacheBust }})

#### Eurocircuits

- [Eurocircuits Zip]({{ "export/AstraControlPower-Eurocircuits.zip" | absolute_url | append: cacheBust }})
- [Eurocircuits BOM CSV]({{ "export/AstraControlPower_bom_Eurocircuits.csv" | absolute_url | append: cacheBust }})
- [Eurocircuits CPL CSV]({{ "export/AstraControlPower_cpl_Eurocircuits.csv" | absolute_url | append: cacheBust }})

#### 3D Step

- [3D Step]({{ "/AstraControlPower-3D.step" | absolute_url | append: cacheBust }})
  
## Report

#### ERC

{% include_relative erc_validation.md %}

#### DRC

{% include_relative drc_validation.md %}

{% include_relative AstraControlPower-report.md %}

## Know Issues

- TBD

## Credits

[KiCad EDA](https://www.kicad.org)

[KiBot](https://github.com/INTI-CMNB/KiBot)

[Amulet - Inspiration for awesome schematic and PCB](https://github.com/EPFLXplore/XRE_LeggedRobot_HW)

[tracespace view - Online Gerber Viewer](https://tracespace.io)