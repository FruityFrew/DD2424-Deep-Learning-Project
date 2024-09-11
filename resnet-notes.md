# ResNet E -- Tests-Performance Table

### Binary classifier
| Learning rate | Epochs | Image transformer settings | Results | Notes |
|:-------------:|:------:|----------------------------|---------|-------|
| 5e-5 | 25 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.65% | |
| 5e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.19%,99.12%,99.05% | |
| 5e-5 | 10 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.78% | |
| 5e-5 | 10 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.78% | |
| 5e-5 | 18 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.58% | |
| 3e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.39%,99.46%,98.92% | |
| 1e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.92% | |
| 4e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.12% | |


### Multi-class classifier
| Learning rate | Epochs | Image transformer settings | Results | Notes |
|:-------------:|:------:|----------------------------|---------|-------|
| layer4:`1e-4`, fc:`1e-3` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 82.89% | |
| fc:`1e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 79.24% | |
| fc:`1e-5` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 53.14% | |
| fc:`1e-3` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 80.87% | |
| fc:`5e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 80.66% | |
| fc:`5e-4` | 40 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 80.73% | |
| layer4:`5e-5`, fc:`5e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 82.76% | |
| layer4:`5e-4`, fc:`5e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 79.78% | |
| layer4:`1e-4`, fc:`5e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 83.98% | |
| layer3:`1e-4`, layer4:`5e-5` | 10 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 95.22% | |
| layer3:`1e-4`, layer4:`5e-5` | 17 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 96.30% | |
| layer3:`1e-4`, layer4:`5e-5` | 25 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 95.31% | |


### Multi-class classifier by ziyi

| Learning rate | Epochs | Image transformer settings | Results | Notes(infer time) |
|:-------------:|:------:|----------------------|---------|-------------------|
|   fc:`5e-5`   |   10   | ViT+Lora             | 96.75%  | 4.48s             |
|   fc:`1e-5`   |   10   | ViT+Lora             | 2.97%   | 5.08s             |
|   fc:`3e-5`   |   10   | ViT+Lora             | 94.32%  | 5.26s             |
|   fc:`5e-5`   |   20   | ViT+Lora             | 97.63%  | 4.75s             |
|   fc:`1e-5`   |   20   | ViT+Lora             | 86.41%  | 4.81s             |
|   fc:`3e-5`   |   20   | ViT+Lora             | 97.35%  | 7.22s             |
|   fc:`1e-5`   |   20   | ViT                  | 90.26%  | 15.22s            |
|   fc:`3e-5`   |   20   | ViT                  | 91.26%  | 16.39s            |
|   fc:`5e-5`   |   20   | ViT                  | 92.26%  | 14.85s            |
