# ICIP_2022
The accepted paper for IEEE International Conference on Image Processing (ICIP2022)

W. Zhou, S. -I. Kamata, Z. Luo and X. Xue, "Rethinking Unified Spectral-Spatial-Based Hyperspectral Image Classification Under 3D Configuration of Vision Transformer," 2022 IEEE International Conference on Image Processing (ICIP), 2022, pp. 711-715, doi: 10.1109/ICIP46576.2022.9897603.(https://ieeexplore.ieee.org/document/9897603)

**Please kindly cite the papers if this code is useful and helpful for your research.**

![image](https://github.com/zhouweilian1904/ICIP_2022/blob/main/whole%20structure.png)

**Abstract:**

Vision Transformer (ViT) has been introduced into the computer vision (CV) field with its self-attention mechanism to capture global dependency. However, simply deploying ViT on a hyperspectral image (HSI) classification task can not get satisfying results because ViT is a spatial-only self-attention model, but rich spectral information exists in HSI. Moreover, most HSI classifiers integrate spectral and spatial features in a cascaded flowchart, ignoring the internal correlation between spectral and spatial information. Furthermore, existing positional embedding (PE) methods can not fulfil the 3D configuration of ViT. Therefore, this paper proposes a unified spectral-spatial-based 3D ViT with cooperative 3D coordinate positional embedding. In the meanwhile, a novel local-global feature fusion strategy is proposed. The model does not contain convolution or recurrent units and can achieve more competitive classification performance than other state-of-the-art (SOTA) methods. Furthermore, compared with existing ViT-based HSI classifiers, our concept can get better results.

--------------------------------
**Datasets:**

We have uploaded several datasets: https://drive.google.com/drive/folders/1IQxuz4jpwf6goB_2ZwVLEZz1ILScymdO?usp=share_link
1. Indian Pines, 
2. PaviaU, 
3. PaviaC, 
4. Botswana, 
5. Houston 2013, 
6. KSC, 
7. Mississippi_Gulfport, 
8. Salinas, 
9. Simulate_database, 
10. Augmented_IndianPines, 
11. Augmented_Mississippi_Gulfport, 
12. Augmented_PaviaU
13. The disjoint datasets (IP, PU, HU) can be referred in https://github.com/danfenghong/IEEE_TGRS_SpectralFormer.


--------------------------------
**How to use:**

you can find and add some arguments in *main.py* for your own testing.

For example:

python main.py --model zhouICIP2022 --dataset IndianPines --training_sample 0.1 --cuda 0 --epoch 200 --batch_size 100 --patch_size 9
