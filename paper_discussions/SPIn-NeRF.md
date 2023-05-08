# Discussion on "SPIn-NeRF: Multiview Segmentation and Perceptual Inpainting with Neural Radiance Fields"

## Questions

Q1. noticed that you have a MVSeg folder in the released source code and we suspect that it was used to extract the masks. But we can't find any info regarding how to run it in the readme file. So can you explain what's the purpose of MVSeg in the project and how you run this module, and how it's integrated in the whole pipeline?

Answer: About the MVSeg folder, it already contains the source code for multiview segmentation, and I'll soon add the description about how to run it to the repository

Q2. would like to know about details about inpainting. Is there any special requirement for the background of the area to be in-painted? For instance, if multiple repeated objects exist in the scene, and we only inpaint one of them, would the result be good? Or if all of them are inpainted, what's to be considered for their background.

A: About the background question, the simpler the background is, the better the results are going to look like. In general, LaMa, the 2D inpainter used in our work, is mostly good at inpainting textures, and not generating new  concepts. SPIn-NeRF would still work with more complex scenes with various occlusions, but I suspect the quality is best when the background needs texture-like inpaintings. We see the quality improvements for various scene scenarios as an exciting avenue for future work. 

Q3. What about the dynamic scene application of SPIn-NeRF, what's your consideration on the application on dynamic scenes?

A: About dynamic scenes, that wasn't our focus, and the same approach wouldn't be directy available to dynamic scenes. Worthwhile to mention, you would be able to get OK-ish results by applying SPIn-NeRF to dynamic scenarios, but to apply it to dynamic scenes, the approach would need some changes and improvements, which is again an interesting direction for follow-up works. 