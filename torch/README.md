# How to build this example

This example uses Torch library (http://torch.ch). You can get a copy of Torch library from pytorch. 

```
git clone https://github.com/pytorch/pytorch.git
cd tools/torch/lib/TH
mkdir build
cd build
cmake ..
make
make install
```
Once TH library is installed, run in this example's directory:
```
ghc -O -lTH -L<path_to_pytorch>/pytorch/torch/lib/TH/build --backpack simple.bkp
```
then
```
main/Main
```

`Tensor=int-tensor:Tensor` can be changed to `Tensor=float-tensor:Tensor`, then the result would become `440.0` instead of `440`
