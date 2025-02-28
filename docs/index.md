## 📂 Dataset Structure

The dataset is organized as follows:
```plaintext
SemanticRail3D/
                ├── train_part1/
                │   ├── cloudXXX_SegY/
                │   │   ├── coord.npy
                │   │   ├── intensity.npy
                │   │   ├── normal.npy
                │   │   ├── feature.npy
                │   │   ├── color.npy
                │   │   ├── instance.npy
                │   │   ├── segment.npy
                │   ├── cloudXXX_SegY/
                │   ├── ...
                ├── train_part2/
                ├── train_part3/
                ├── train_part4/
                ├── train_part5/
                │
                ├── Validation/
                │   ├── cloudXXX_SegY/
                │   ├── ...
                │
                ├── Test/
                │   ├── cloudXXX_SegY/
                │   ├── ...
