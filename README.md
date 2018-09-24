# MABE_Vis

Public repository for visualization code related to [Modular Agent Based Evolution Framework](https://github.com/Hintzelab/MABE) (aka MABE).

The intention behind this repo is to aid code reuse. In many experiments the part of the code that does graphics usually requires the most work. It is often too messy to be submitted to the main repository, so it is also the part that tends to be shared between the developers the least and is most frequently rewritten as a result. The purpose of this repository is to change that.

We accept all programs that can potentially be useful in visualizing any MABE-related entities such as Worlds, Brains or Optimizers. Codes that visualize other aspects of MABE operation (such as interaction between the components) are accepted as well. No further requirements are placed on the code, meaning that it can
* be written in any language for any OS;
* use any coding and formatting style;
* have any degree of compatibility with the current version of MABE;
* have any amount of comments and documentation, including no comments or documentation whatsoever;
* be incomplete and/or inoperative.

In short, if you wrote a visualization code for any of the systems involved in MABE, you're welcome to submit it. If your code wasn't developed in the context of MABE, but involved any systems that MABE supports (including modules available from [MABE_extras](https://github.com/Hintzelab/MABE_extras) and external forks), you're still welcome to submit it.

Depending on the type the code you submit, it can be reused or used as a starting point or as a guideline for some new visualization tool for MABE.

## Contributing

There are two ways to contribute:

1. Submit your code directly to the repository through a pull request (see the instructions below).
2. Email your code to `abernats at uvm.edu` and I'll take care of it.

Regardless of how you submit, any supplementary comments and/or instructions for the code are welcome. If your code requires MABE to be modified to work, please include the changes (the changed files or a patch) if you have them available.

To make a pull request to the repository, follow these steps:

1. Note the path where your code should be stored : `<codeType>/<mabeModulePath>/<visualizationName>`.

   `codeType` is determined as follows:
   - if your code is compatible with the stable version of MABE and thoroughly tested, it should be classified as *stable*.
   - if your code is compatible with MABE, but not in its stable version and/or is not tested much, it is *experimental*.
   - in all other cases the code is *raw*.

   `mabeModulePath` is the path in the folder hierarchy of [the stable MABE version](https://github.com/Hintzelab/MABE) to where your module normally resides.

   `visualizationName` is the name of your code.

   For example, suppose you made a visualizer that draws something equivalent to MABE's BerryWorld, but is not compatible with the current version of MABE. Suppose further that you called it glBerryEaters, then your path would be `raw/World/BerryWorld/glBerryEaters`.

2. Fork [this repository](https://github.com/Hintzelab/MABE_Vis.git) to your Github account.

3. Create the folder for your code using the path determined in step 1, place your code there and add it to git (e.g. by typing `git add -A`).

4. Push your changes to your fork and [create a pull request](https://help.github.com/articles/creating-a-pull-request/).
