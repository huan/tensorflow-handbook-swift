# Tensorflow in Swift

[![Build Status](https://travis-ci.com/huan/tensorflow-handbook-swift.svg?branch=master)](https://travis-ci.com/huan/tensorflow-handbook-swift)

![Swift for Tensorflow](docs/images/swift-tensorflow.png)

This repository is the [Swift Chapter](https://tf.wiki/zh/appendix/swift.html) for [简单粗暴TensorFlow | A Concise Handbook of TensorFlow](https://tf.wiki)

MNIST Example in Book: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huan/tensorflow-handbook-swift/blob/master/swift-for-tensorflow-mnist-example.ipynb)

Book Chapter: Tensorflow Handbook - Swift

- Github Repository: <https://github.com/huan/tensorflow-handbook-swift>
- Github Pages: <https://huan.github.io/tensorflow-handbook-swift/>

## USAGE

### For those who had Swift installed

If you had installed Swift locally, then you can run swift directly:

```shell
$ swift run
Downloading train-images-idx3-ubyte ...
Downloading train-labels-idx1-ubyte ...
Reading data.
Constructing data tensors.
Test Accuracy: 0.9116667
```

### For those who had no Swift installed (Docker)

If you are using Windows, or Ubuntu 19 (Swift for Tensorflow only supports Mac & Ubuntu 18.04 at Aug 2019), then the only way which you can play with this repository is to use Docker.

```shell
# use `nvidia-docker` if you want to use GPU
docker run -ti --rm \
  --privileged \
  --userns=host \
  -v "$(pwd)":/notebooks \
  zixia/swift \
  swift run
```

See:

1. Docker parameters - <https://github.com/hashicorp/nomad/issues/1904#issuecomment-523295864>
1. Docker Repo of `zixia/swift` - <https://github.com/huan/docker-swift-tensorflow>

## TODO

## RESOURCES

- [Colab notebooks for Swift for TensorFlow](https://github.com/zaidalyafeai/Swift4TF)
- [fast.ai Embracing Swift for Deep Learning](https://www.fast.ai/2019/03/06/fastai-swift/)
- [High Performance Numeric Programming with Swift: Explorations and Reflections](https://www.fast.ai/2019/01/10/swift-numerics/)
- [Swift for TensorFlow Design Overview](https://github.com/tensorflow/swift/blob/master/docs/DesignOverview.md)

### Videos

- [Swift for TensorFlow (TensorFlow @ O’Reilly AI Conference, San Francisco '18)](https://www.youtube.com/watch?v=mu0j4Gd2YY8)
- [Swift for TensorFlow: The Next-Generation Machine Learning Framework (TF Dev Summit '19)](https://www.youtube.com/watch?v=s65BigoMV_I)

## Author

[Huan](https://github.com/huan) [(李卓桓)](https://linkedin.com/in/zixia) \<zixia@zixia.net\>

<a href="http://stackoverflow.com/users/1123955/zixia">
  <img src="http://stackoverflow.com/users/flair/1123955.png" width="208" height="58" alt="profile for zixia at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for zixia at Stack Overflow, Q&amp;A for professional and enthusiast programmers">
</a>

## Copyright & License

- Code & Docs © 2018 - now Huan (李卓桓) \<zixia@zixia.net\>
- Code released under the Apache-2.0 License
- Docs released under Creative Commons
