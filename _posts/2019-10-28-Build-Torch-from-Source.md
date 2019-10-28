---
title: "Building Torch from Source"
layout: post
date: 2019-10-28 14.00
tag: [C++, Torch, Deep Learning]
headerImage: true
projects: true
# hidden: true # don't count this post in blog pagination
category: goksu
author: goksuguvendiren
externalLink: false
---

## Building Torch from Source

Recently I've needed to use the C++ interface of Torch, and am actually surprised to see how little information is out there about everything related to it. Everything I've found is pretty much what I've found through forums and questions bit by bit. Even for building it from the source doesn't have a documentation. The README in the github page explains the usage of a setup script, but I ended up not being able to run it. Then you just have to somehow figure it out another way to build it. 

Although so far it looks trivial to build it with prior knowledge on *git* and *CMake*, it would save me some time if there were some documentation explaining step by step. This page is for my own future reference, but you're welcome to correct me if you see something that can be improved.

So, here goes. First, let's get the source from the GitHub: 

``` 
git clone git@github.com:pytorch/pytorch.git
```

This only brings the source for Torch. You need to pull the submodules it uses. 
But first, go into the directory of Torch.

``` 
cd pytorch
git submodule sync
git submodule update --init --recursive
```

Now, let's create a directory for the build artifacts, and build from there.

```
mkdir build
cd build
cmake ..
make -j12
sudo make install
```

After these steps, you should have the library ready. After this point, if you want to further personalize the build settings, I suggest you use __ccmake__ to see the options that you can adjust, and build with those settings.

### Troubleshooting

* If you have g++ version greater than 6.0, and CUDA 9.0-9.2, you need to either upgrade your CUDA version, or downgrade compiler version. These are already prompted as an error by the cmake, as well as a solution to it:
```
export CUDACXXHOST='/usr/bin/g++-5'
``` 
But do not forget to cleanup the CMake cache before rerunning the CMake, because those variables are cached, you'll end up with the same error!

* ```nvcc fatal : Unsupported gpu architecture 'compute_75'```.
Apparently, your device supports a higher compute capability than your CUDA version. Seems that CUDA 9.2 supports only compute capability 7.0 and 7.2, so doing this should solve the problem:
```
export TORCH_CUDA_ARCH_LIST="7.0"
```