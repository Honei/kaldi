# 这个是自己看kaldi笔记，同时也是给了很多注释
## 最开始是从看声纹识别开始，从MFCC特征提取到GMM

[![Build Status](https://travis-ci.com/kaldi-asr/kaldi.svg?branch=master)](https://travis-ci.com/kaldi-asr/kaldi)
Kaldi Speech Recognition Toolkit
================================
阅读`./INSTALL`了解如何构建整个kaldi的工具包。这些说明适用于UNIX系的系统，包括各种Linux的发行版,Darwin和Cygwin。<br>
阅读`windows/INSTALL`，获得Windows系统的安装说明

<br>
阅读`egs/README.txt`获得运行kalid示例的说明

<br>
If you encounter problems (and you probably will), please do not hesitate to
contact the developers (see below). In addition to specific questions, please
let us know if there are specific aspects of the project that you feel could be
improved, that you find confusing, etc., and which missing features you most
wish it had.

Kaldi information channels
--------------------------

For HOT news about Kaldi see [the project site](http://kaldi-asr.org/).

[Documentation of Kaldi](http://kaldi-asr.org/doc/):
- Info about the project, description of techniques, tutorial for C++ coding.
- Doxygen reference of the C++ code.

[Kaldi forums and mailing lists](http://kaldi-asr.org/forums.html):

We have two different lists
- User list kaldi-help
- Developer list kaldi-developers:

To sign up to any of those mailing lists, go to
[http://kaldi-asr.org/forums.html](http://kaldi-asr.org/forums.html):


Development pattern for contributors
------------------------------------

1. [Create a personal fork](https://help.github.com/articles/fork-a-repo/)
   of the [main Kaldi repository](https://github.com/kaldi-asr/kaldi) in GitHub.
2. Make your changes in a named branch different from `master`, e.g. you create
   a branch `my-awesome-feature`.
3. [Generate a pull request](https://help.github.com/articles/creating-a-pull-request/)
   through the Web interface of GitHub.
4. As a general rule, please follow [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html).
   There are a [few exceptions in Kaldi](http://kaldi-asr.org/doc/style.html).
   You can use the [Google's cpplint.py](https://raw.githubusercontent.com/google/styleguide/gh-pages/cpplint/cpplint.py)
   to verify that your code is free of basic mistakes.

Platform specific notes
-----------------------

### PowerPC 64bits little-endian (ppc64le)

- Kaldi is expected to work out of the box in RHEL >= 7 and Ubuntu >= 16.04 with
  OpenBLAS, ATLAS, or CUDA.
- CUDA drivers for ppc64le can be found at [https://developer.nvidia.com/cuda-downloads](https://developer.nvidia.com/cuda-downloads).
- An [IBM Redbook](https://www.redbooks.ibm.com/abstracts/redp5169.html) is
  available as a guide to install and configure CUDA.

### Android

- Kaldi supports cross compiling for Android using Android NDK, clang++ and
  OpenBLAS.
- See [this blog post](http://jcsilva.github.io/2017/03/18/compile-kaldi-android/)
  for details.
