# ResNet E -- Tests-Performance Table

### Binary classifier
| Learning rate | Epochs | Image transformer settings | Resutls | Notes |
|:-------------:|:------:|----------------------------|---------|-------|
| 5e-5 | 25 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.65% | |
| 0.00005 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.19%,99.12%,99.05% | |
| 5e-5 | 10 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.78% | |
| 5e-5 | 10 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.78% | |
| 5e-5 | 18 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.58% | |
| 3e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.39%,99.46%,98.92% | |
| 1e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 98.92% | |
| 4e-5 | 20 | `RandomCrop,RandomHorizontalFliop,RandomRotation(15)` | 99.12% | |


### Multi-class classifier
| Learning rate | Epochs | Image transformer settings | Resutls | Notes |
|:-------------:|:------:|----------------------------|---------|-------|
| layer4:`1e-4`, fc:`1e-3` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 82.89% | |
| fc:`1e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 79.24% | |
| fc:`1e-5` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 53.14% | |
| fc:`1e-3` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 80.87% | |
| fc:`5e-4` | 20 | `RandomHorizontalFlip,RandomRotation(10),RandomResizedCrop` | 80.66% | |
