# Audio Spline Plugin

A **Blueprint-Only Plugin** for Unreal Engine that allows an **Audio Component** to move along a **Spline**, following a **Target Actor** dynamically. This plugin is useful for audio effects like moving sounds along a path.

## Features
- **Audio Component moves along a Spline.**
- **Follows a Target Actor dynamically.**
- **Works without C++ (Blueprint-Only).**
- **Easily editable in the Level Editor.**

## Installation

### **1. Install the Plugin**
#### Option 1: Install in Your Project
1. Download or clone the plugin repository.
2. Copy the `AudioSplinePlugin` folder into:
   ```
   YourProject/Plugins/
   ```
3. Open Unreal Engine.
4. Go to `Edit > Plugins`.
5. Find `Audio Spline Plugin` and **enable** it.
6. Restart Unreal Engine.

#### Option 2: Install as an Engine Plugin (Global Install)
1. Copy `AudioSplinePlugin` into your Unreal Engine installation:
   ```
   UnrealEngine/Engine/Plugins/
   ```
2. Restart Unreal Engine.
3. Enable it from `Edit > Plugins`.

## How to Use

### **1. Add BP_AudioSpline to Your Level**
1. Open your Unreal Engine **Level Map**.
2. In the **Content Browser**, go to:
   ```
   Plugins > AudioSplinePlugin > Content
   ```
3. Drag `BP_AudioSpline` into your level.

### **2. Create and Edit the Spline**
1. **Select `BP_AudioSpline` in the Level.**
2. In the **Details Panel**, locate `SplineComponent`.
3. **Hold `ALT` + Drag** an existing spline point to create more.
4. Move spline points to adjust the path.

### **3. Set the Target Actor**
1. In **BP_AudioSpline’s** **Details Panel**, find the `Target` variable.
2. Assign an **Actor** (e.g., a moving player, enemy, or object).

### **4. Play Sound Along the Spline**
1. Assign a **Sound** to `AudioComponent`.
2. Set **Auto-Activate = true** or call `Play` from Blueprint.

## Advanced Customization
- Modify `SplineComponent` settings to adjust curve tension.
- Adjust `AudioComponent` properties to control volume, spatialization, or reverb effects.
- Use Blueprint logic to dynamically change the `Target` actor at runtime.
