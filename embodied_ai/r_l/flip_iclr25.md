template is here
# Paper Title: *[FLIP: FLOW-CENTRIC GENERATIVE PLANNING FOR GENERAL-PURPOSE MANIPULATION TASKS]*  
**Authors**: [Prof shao lin , nus]  
**Published In**: [iclr2025, 866]  

---

## 1. Summary
- **Problem Addressed**: 
1. generates image flows (future trajectories on query points) as actions for planning.
2.  flow-conditioned video generation network D generates the following L frames based on current image observation history, the language goal g, and the predicted flow
pt:t+L to enable iterative planning for the next planning step.
3.  The value module V assigns an estimated value V t for each frame ot to enable model-based planning on the image space.

![这是图片](/embodied_ai/r_l/imgs/FLIP_iclr25.jpeg "frame")



## 3. Key Takeaways
- language-img similarity 可以做value /reward很有新意
- 相比于ATM,RSS,pieter abbeel，这篇工作用image flow替换了point tracking。不不不 还是point tracking。 这篇工作预测位移而不是绝对位置，有performance boost.
-  planning through beam search with reward from video-language reward
