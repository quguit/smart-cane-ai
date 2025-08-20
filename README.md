# Smart Cane AI

An AI-powered smart cane system to assist stroke patients during rehabilitation.  
The system monitors gait patterns and helps track recovery or detect deterioration over time.  

## Goals
- Collect gait data from sensors (accelerometer, gyroscope, etc.)
- Analyze and classify walking patterns
- Differentiate between healthy and impaired gait
- Provide long-term monitoring for stroke rehabilitation

## Project Structure
- `docs/` → project documentation and research notes  
- `data/` → datasets or dataset links  
- `notebooks/` → experiments and prototyping  
- `src/` → source code for preprocessing and AI models  
- `tests/` → unit and integration tests  

## Next Steps
1. Research available gait datasets  
2. Define clinically relevant gait parameters  
3. Build preprocessing pipeline  
4. Train initial AI model  

---
*This project is under development. Contributions and ideas are welcome!*


# Next step

## Clinical Gait Features

Instead of relying only on raw sensor data, this project extracts **clinical gait features** from accelerometer and gyroscope signals.  
These features are widely used in rehabilitation and gait analysis, and allow the AI model to detect meaningful differences between healthy and impaired walking patterns.

### Implemented Features
- **Step Time** – average time between steps (slower and more variable in stroke patients)  
- **Cadence** – number of steps per minute (indicator of walking speed and endurance)  
- **Step Length Variability** – irregularity in step size, often linked to instability  
- **Gait Symmetry** – balance between left and right steps (asymmetry is common after stroke)  
- **Step Regularity** – consistency of step cycles, measured via autocorrelation  
- **Harmonic Ratio** – stability of gait pattern in the frequency domain  

### Advantages
- Transforms raw sensor signals into **clinically interpretable metrics**  
- Enables **objective monitoring** of patient progress over time  
- Helps clinicians distinguish between **improvement, deterioration, or abnormal gait events**  
- Provides a compact and informative feature vector for AI models, reducing noise and improving accuracy
