# WorldModels_List

### [GigaWorld-0: World Models as Data Engine to Empower Embodied AI]

- **[Paper](https://arxiv.org/pdf/2511.19861)**
- **[Code](https://github.com/open-gigaai/giga-world-0)**
- **Summary**:
  - **Video Module**
    - *Video-Dreamer* based on:
      - Flow Matching
      - DiT with Sparse Attention
      - Mixture-of-Experts (MoE)
    - Supports controllable generation (appearance, viewpoint, action)
  
  - **3D Module**
    - Builds geometry-aware scenes
    - Learns **physical parameters** (e.g., friction, stiffness)
    - Ensures **physics consistency**
- #### Pipeline:
    Text / Image → Video Model (generate visual dynamics) → Inverse Dynamics Model (infer actions) → 3D World Modeling (enforce geometry + physics) → Generated Data: (video, action) → Train VLA policy
