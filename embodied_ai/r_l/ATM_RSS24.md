template is here
# Paper Title: *[Any-point Trajectory Modeling for Policy Learning]*  
**Authors**: [Pieter Abbeel]  
**Published In**: [rss2024]  

---

## 1. Summary
- **Problem Addressed**: 
1. first stage : predict the future points give a frame in a video. The points are uniform grid sample. The model is an auto-regressive transformer. The loss is multi-modal masked prediction loss.
2. second stage: train a policy(could be MLP/ diffusion) to prediction future actions given current image and predicted tracking points. The MSE Loss is used. This stage is imatation learning.
![这是图片](/embodied_ai/r_l/imgs/atm_rss2024.png  "main_arch")
![这是图片](/embodied_ai/r_l/imgs/atm_rss2024_2.png  "policy ")




## 3. Key Takeaways
- Q: why need points ---> points guide policy training, points are efficient than imgs, video prediction are redundant.

