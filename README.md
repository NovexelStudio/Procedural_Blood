# Procedural_Blood
Procedural Blood Shader (Unity Shader Graph)
Procedural Blood Shader (Unity Shader Graph)

This project implements a fully procedural blood decal shader in Unity using Shader Graph. It creates dynamic blood splatter effects without relying on external textures, making it efficient and highly customizable for any surface or lighting condition.

🧠 Overview

The shader procedurally generates a blood pattern using layered noise, gradient masks, and adjustable parameters. It can be used with Unity’s Decal Projector or as a material on meshes and surfaces.

⚙️ Features

Procedural Generation: No texture maps required.

Customizable Controls:

Size – overall splatter scale.

Sharpen – controls edge definition.

Color – base blood color.

Noise Scale – controls pattern density.

Noise Amp – adjusts the depth/intensity of variation.

Noise Offset – animates or randomizes splatter shape.

Dynamic Falloff: Smooth radial gradient blends edges naturally.

Noise-Based Irregularity: Layered noise simulates natural splatter and pooling.

🧩 Technical Details

The graph combines UV gradients to form a radial mask, then distorts it with two noise layers. The noise output is sharpened to define splatter boundaries and modulated with the user’s color input. The final alpha is controlled by a radial falloff mask for realistic blending.

🚀 Use

Create a new Shader Graph (URP/HDRP compatible).

Copy the node structure shown in the included screenshot.

Create a Material using this shader and apply it via a Decal Projector or directly on geometry.

Adjust parameters in real time to generate unique splatter patterns.

🩸 Result

A reusable, lightweight blood effect that adapts procedurally—no repeated textures, no extra memory overhead, and fully tweakable in-editor.
