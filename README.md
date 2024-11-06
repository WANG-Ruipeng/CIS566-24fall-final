# CIS 5660 Final Project

Team members: Sirui Zhu, Crystal Jin, Ruipeng Wang

## Project planning: Design Doc (due 11/6)

### Design Doc

### Introduction

Chinese architecture is renowned for its unique and enduring aesthetic, deeply rooted in cultural symbolism and harmony with nature. Among the many regional styles, **Jiangnan architecture**—popular in the southern Yangtze River region—stands out for its elegance and simplicity. Characterized by **white walls and black-tiled roofs**, Jiangnan buildings capture a distinct visual appeal that balances sophistication with natural surroundings.

This project aims to recreate the essence of Jiangnan buildings through procedural generation, focusing on elements like the iconic roof curves, wall textures, and subtle detailing. By exploring these forms and patterns, we hope to capture the serene and harmonious qualities that define this celebrated style.

### Goal

The aim of this project is to create a procedural generator that produces traditional Jiangnan-style buildings, inspired by the visual aesthetics of 江南百景图 or *Jiangnan Hundred Scenes*. Through this project, we intend to:

1. **Reproduce Authentic Architectural Details**: Develop a system that generates white-walled, black-tiled structures characteristic of Jiangnan architecture, capturing the simplicity and harmony of the region’s unique aesthetic. This includes features such as upturned roof eaves, ornate wooden lattice windows, and traditional courtyards.
2. **Facilitate Dynamic Environment Creation**: Design a generator that allows for quick and dynamic placement of Jiangnan-style buildings and elements within a scene. This flexibility will support the creation of varied environments that mimic the distinct neighborhoods and picturesque layouts seen in *Jiangnan Hundred Scenes*.
3. **Enable Customization and Interactivity**: Allow users to customize various architectural features, such as building height,  plant types and city layout. These customization options will make it easy to create a variety of traditional Chinese buildings while maintaining the artistic and historical essence of the Jiangnan style.

By achieving these objectives, we hope to deliver a tool that not only embodies the beauty of Jiangnan architecture but also allows for creative freedom in designing environments reminiscent of *Jiangnan Hundred Scenes*.

### Inspiration/reference:

![Google Playstore](https://play.google.com/store/apps/details?id=com.cis.jiangnan.googleplay)

![Link to description](https://shouyou.3dmgame.com/zt/106370_gl_all_44/)

![image.png](image.png)

![image.png](image%201.png)

![image.png](image%202.png)

### Specification:

- Procedural generated items list:
    - Two types of trees:
        - willow
        - plum blossom
    - Four types of houses:
        - residential building
        - shops
        - pavilion
        - tower
    - River
        - with/without lotus
    - Road
        - Brick
        - Stone
    - Bridge/Boat
- Water painting stylization

### Techniques

We plan to use **Unity** and the **Wave Function Collapse (WFC)** algorithm to procedurally generate Jiangnan-style architecture. WFC is well-suited for arranging elements based on sample patterns.

1. **Unity**: Unity will serve as our primary platform, enabling real-time adjustments and modular design of architectural elements like walls, roofs, and courtyards.
2. **Wave Function Collapse Algorithm**: WFC will guide the placement of architectural components by referencing Jiangnan-style patterns, ensuring visually coherent and varied outputs.

[https://robertheaton.com/2018/12/17/wavefunction-collapse-algorithm/](https://robertheaton.com/2018/12/17/wavefunction-collapse-algorithm/)

[https://github.com/mxgmn/WaveFunctionCollapse](https://github.com/mxgmn/WaveFunctionCollapse)

### Design

- **Input Pattern Module → WFC Module → Element Modules → Scene Assembly Module**
- **User Interface Module** interacts with **WFC Module** for real-time adjustments.

### Timeline

| Week | Task | Crystal Jin | Sirui Zhu | Ruipeng Wang |
| --- | --- | --- | --- | --- |
| **Week 1** | Initial Setup & Basic Module Creation | Set up Unity project and WFC integration, design base procedural logic | Begin designing prefabs for houses and roads | Design prefabs for trees and water elements |
| **Week 2** | Implement Core Generation Features | Develop procedural rules for house types (residential, shops, pavilion, tower) | Integrate roads (brick, stone) and bridges, basic scene composition | Implement river with lotus options, basic tree placement (willow, plum blossom) |
| **Week 3** | Water Painting Stylization & Customization | Implement water painting shader stylization | Add UI for selecting item types (houses, trees, roads) | Refine procedural generation for variety and realism (item size, spacing) |
| **Week 4** | Final Assembly & Polish | Integrate all elements in scene, optimize generation | Apply final visual adjustments and scene lighting | Conduct testing, debug procedural issues, and prepare for final presentation |
