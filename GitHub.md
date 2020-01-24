# GitHub Contributions

By far, my favorite part of Google Code-in with TensorFlow was contributions through GitHub. Below are some of the repositories that I contributed to. Note that not all of these had to do with tasks - a big part of GCI is community involvement :heart:

## Pull Requests
Pull Requests are my most direct contributions to TensorFlow.
- [SwiftPlot](https://github.com/KarthikRIyer/swiftplot/pulls/WilliamHYZhang)
- [TensorFlow Core](https://github.com/tensorflow/tensorflow/pulls/WilliamHYZhang)
- [TensorFlow Datasets](https://github.com/tensorflow/datasets/pulls/WilliamHYZhang)
- [TensorFlow Examples](https://github.com/tensorflow/examples/pulls/WilliamHYZhang)
- [Swift Jupyter](https://github.com/google/swift-jupyter/pulls/WilliamHYZhang)
- [Swift-Models](https://github.com/tensorflow/swift-models/pulls/WilliamHYZhang)

## Issues
I also created some issues that I helped find/solve.
- [SwiftPlot](https://github.com/KarthikRIyer/swiftplot/issues/WilliamHYZhang)
- [TensorFlow Datasets](https://github.com/tensorflow/datasets/issues/WilliamHYZhang)

## Code Review / Discussion
I really enjoyed helping my fellow GCI peers out whenever I could.
- [SwiftPlot](https://github.com/KarthikRIyer/swiftplot/pulls?utf8=%E2%9C%93&q=commenter%3AWilliamHYZhang+-author%3AWilliamHYZhang)
- [TensorFlow Core](https://github.com/tensorflow/tensorflow/pulls?utf8=%E2%9C%93&q=commenter%3AWilliamHYZhang+-author%3AWilliamHYZhang)
 - [TensorFlow Datasets](https://github.com/tensorflow/datasets/pulls?utf8=%E2%9C%93&q=commenter%3AWilliamHYZhang+-author%3AWilliamHYZhang)
 - [TensorFlow Examples](https://github.com/tensorflow/examples/pulls?utf8=%E2%9C%93&q=commenter%3AWilliamHYZhang+-author%3AWilliamHYZhang)
 - [Swift-Models](https://github.com/tensorflow/swift-models/pulls?utf8=%E2%9C%93&q=commenter%3AWilliamHYZhang+-author%3AWilliamHYZhang)

## S5TF Team
The current state of datasets in `swift-models` is described as follows from the GitHub conversation [here](https://github.com/tensorflow/swift-models/issues/253):

Brad Larson:

> The "datasets" that we have in the repository are more like wrappers around the actual datasets, and right now they provide the minimal functionality needed to feed data into the (largely image classificaion) models we use for testing. The ones that have been set up in here were chosen for their ability to exercise common network architectures.

> I agree, there's a lot to like about the tensorflow/datasets library, and we've had a number of conversations with that team. We'll be talking more about the dataset design soon, but for right now these exist in the service of the models in the repository, which is why they remain here.

Brennan Saeta:

> I really like https://github.com/tensorflow/datasets and think a Swift-flavored variation of that would fit in very well in this (swift-models) repository. (Concretely, having fewer repositories means it's easier to see how things fit together because there can be a sample program that combines a pre-built model architecture with a pre-built dataset together into an example program.)

The S5TF team (myself and fellow GCI competitor Rick Wierenga) has recognized this and are currently actively working on developing the foundations for a new datasets API for using with Swift for TensorFlow. The skeletal api structure has already been built (based off of TFDS), with the implementation of MNIST almost complete. Check it out [here](https://github.com/s5tf-team/datasets).

The S5TF team also has a great [example notebook](https://github.com/s5tf-team/examples) in lieu of their own `S5TFDatasets` API. The notebook demonstrates how to take TFDS datasets, load them in Swift through Python interoperability, and with a little coaxing convert them from `PythonObject`s into usable `Tensor`s that you can pass into the model.
