# CIS 5660 Final Project

Team members: Sirui Zhu, Crystal Jin, Ruipeng Wang

This repository will **NOT** contain actual assets and code in our Unity project because we used some purchased assets.

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

[Google Playstore](https://play.google.com/store/apps/details?id=com.cis.jiangnan.googleplay)

[Link to description](https://shouyou.3dmgame.com/zt/106370_gl_all_44/)

![image.png](ReadmeFiles/image.png)

![image.png](ReadmeFiles/image%201.png)

![image.png](ReadmeFiles/image%202.png)

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

- **Maya** -> **Photoshop for textureing** -> **Unity**
- **User Interface Module** interacts with **WFC Module** for real-time adjustments.

### Timeline

| Week | Task | Sirui Zhu | Crystal Jin | Ruipeng Wang |
| --- | --- | --- | --- | --- |
| **Week 1** | Initial Setup & Basic Module Creation | Set up Unity project and WFC integration, design base procedural logic | Begin designing prefabs for houses and roads | Design prefabs for trees and water elements |
| **Week 2** | Implement Core Generation Features | Develop procedural rules for house types (residential, shops, pavilion, tower) | Integrate roads (brick, stone) and bridges, basic scene composition | Implement river with lotus options, basic tree placement (willow, plum blossom) |
| **Week 3** | Water Painting Stylization & Customization | Implement water painting shader stylization | Add UI for selecting item types (houses, trees, roads) | Refine procedural generation for variety and realism (item size, spacing) |
| **Week 4** | Final Assembly & Polish | Integrate all elements in scene, optimize generation | Apply final visual adjustments and scene lighting | Conduct testing, debug procedural issues, and prepare for final presentation |

---

## Milestone #1

### Progress Description

So far, we have made significant progress toward our project goals:

1. **Asset Creation**: We created foundational assets tailored to the Jiangnan architectural style. This includes both self-modeled assets and modified free assets from online sources, which have been adjusted to match the aesthetic of traditional Chinese elements.
2. **Grid-Based Wave Function Collapse (WFC) Implementation**: We’ve developed the core grid-based WFC code, which sets the groundwork for procedural generation in our project. Our generator currently uses a grid-based approach, where each tile is influenced by its neighboring tiles based on predefined rules.
3. **Generation Rules Configuration**: We configured specific generation rules, ensuring that each object in the scene adheres to a rule set that determines its allowable neighbors. This configuration enables the generation of coherent, traditional-style layouts, where every element respects the Jiangnan architectural style.

### Current Challenges

We encountered some challenges, mainly with the configuration of WFC rules for complex assets. Each asset requires specific neighbor configurations, which is time-intensive. However, the process has been manageable so far, and we are exploring ways to automate or simplify neighbor rule setup for more efficient generation.

### Demo Output

Below are examples of our generator's current output, demonstrating early but promising results in creating Jiangnan-inspired layouts. The visuals are still in a basic form, as we focused primarily on core functionality rather than detailed polish.

![image.png](ReadmeFiles/image%203.png)

*Buildings & roads*

https://github.com/user-attachments/assets/f8111741-6960-4e32-b9ad-674ac505e9ab

---

## Milestone #2

### Progress Update

Since the completion of Milestone #1, we have made significant improvements to our project:

1. **Smarter Generation Rules**:  
   Our generation rules have become more intelligent. We have implemented functionality to adjust the weights between houses and roads, allowing us to control whether the final generation features more houses or roads.

2. **Post-Processing Effects**:  
   We added several shaders to enhance the overall environment with post-processing effects, achieving the Chinese ink painting aesthetic we envisioned.

3. **Improved Texturing**:  
   The textures of the original houses were updated to better prepare them for final refinement with post-processing. Additionally, we added a river to enrich the scene.

4. **Peer Review Feedback**:  
   During the peer review session, we received valuable suggestions, including:
   - Adding an **FPS mode** to enable players to tour around the procedurally generated city.
   - Enhancing the **river shader** to incorporate more dynamic elements.
   - Improving the interaction between rivers and roads, such as automatically generating bridges when roads intersect with rivers.

### Demo Output

![image.png](ReadmeFiles/Milestone%202.png)

![42821733328357_ pic](https://github.com/user-attachments/assets/f94eafd2-5afd-4437-8ba1-fd6b923066a5)

![42771733326302_ pic](https://github.com/user-attachments/assets/02299795-4f69-4ad0-ab70-ea35dfd91e21)

---

# Milestone #3

## Progress Update

For Milestone #3, our focus was on improving user interactivity, refining the procedural generation logic, and enhancing the overall visual and functional aspects of the project. A key feature introduced is a streamlined **editing tool**, which allows users to manually influence the grid layout before the Wave Function Collapse (WFC) algorithm generates the environment. Additionally, we improved the river generation algorithm to create more natural and balanced layouts, avoiding overly dense water features.

## New Features and Improvements

### 1. **Editing Tool for Grid Customization**

- **Purpose**: The editing tool allows users to customize the initial grid layout by placing specific objects before starting the WFC process. This feature bridges manual design and procedural generation, giving users more control over the final output.
- **Implementation**:
    - Users can **select a tile** by hovering over it, with a wireframe highlight showing the currently selected grid cell.
    - Pressing the **Tab key** cycles through available objects (e.g., house, tree, road) to place on the selected tile.
    - **Click and drag** functionality enables users to quickly place multiple objects across the grid.
    - When the grid customization is complete, pressing the **Spacebar** triggers the WFC algorithm to generate the remaining environment based on the user-defined inputs.
- **Outcome**: This intuitive editing tool empowers users to influence the layout while maintaining the procedural generation's adaptability and aesthetic coherence.

### 2. **Improved River Generation Algorithm**

- The river generation algorithm was updated to ensure **more realistic water distribution**:
    - Rivers are only generated when adjacent to an existing water tile, avoiding overly dense or random water placements.
    - This approach creates more natural and visually appealing waterways, contributing to a balanced scene.

### 3. **Refined Procedural Rules**

- **Dynamic Water Adjustments**: Users can now adjuste the "waterness" in the scene, having more or less water generated.
- **Constraint Handling**: Enhanced WFC rules to respect user-defined placements, treating them as hard constraints during generation.
- These refinements improve the coherence and variety of the generated Jiangnan-style environments.

## Workflow

### Step 1: **Edit Mode**

- Begin by customizing the grid layout:
    - Hover over a tile to select it (wireframe highlights the selection).
    - Use the **Tab key** to cycle through object types (e.g., house, tree, road).
    - **Click and drag** to place objects onto multiple grid cells.
- Modify the grid until satisfied with the initial setup.

### Step 2: **Generate Mode**

- Press the **Spacebar** to start the WFC algorithm.
- The algorithm fills the remaining grid cells based on the user-defined layout and procedural generation rules.

### Step 3: **Explore the Results**

- Observe the final generated environment, which combines user customization and procedural randomness to create a coherent Jiangnan-inspired scene.

## Progress Demo

### Editing tool


https://github.com/user-attachments/assets/ec1c99a8-9511-4f59-ae31-fc6136304ea0


### Waterness index
| 0.1 waterness | 0.9 waterness |
| --- | --- |
| ![image.png](ReadmeFiles/M3_1.png) | ![image.png](ReadmeFiles/M3_2.png) |

---

# Final
## Progress Update
For the final milestone, we focused on enhancing the visual fidelity of our procedurally generated Jiangnan-style buildings by introducing a set of new, carefully curated textures. These textures were designed to align more closely with the aesthetics of our original inspiration：

## Demo Video

https://github.com/user-attachments/assets/b474b98f-cf2f-488d-b931-e7551d310e75

---

## Reference

[CC ROI - STE DreamBigger Photoshop VID 16x9 English](https://www.youtube.com/watch?app=desktop&v=Jsc3BQaJndQ)
