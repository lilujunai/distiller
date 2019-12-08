## Python Dependencies
This codebase only supports Python3.6+.
Required packages:
- `torch torchvision tqdm numpy pandas seaborn` for matrix operations

All packages can be installed using `pip3 install --user -r   requirements.txt`.

## Run
The benchmarks can be run via `python3 evaluate_kd.py` and providing respective command line parameters. For example:

`python3 evaluate_kd.py --epochs 200 --teacher resnet18 --student resnet8  --dataset cifar10 --teacher-checkpoint pretrained/resnet18_cifar10_95260_parallel.pth --mode nokd kd`

Runs basic student training and knowledge distillation for 200 epochs using a
pretrained teacher.


## Supported distillation modes