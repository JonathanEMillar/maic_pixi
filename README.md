# MAIC Pixi environment

![Pymaic Test](https://github.com/JonathanEMillar/maic_pixi/actions/workflows/pymaic-test.yml/badge.svg)

This is a [Pixi](https://pixi.sh) environment that allows you to configure you're machine to run MAIC.

## Prerequisites

* Python 3.8 or higher
* Git
* Pixi (for environment and dependency management)

## Installation

1. Install Pixi on your own machine:

```
curl -fsSL https://pixi.sh/install.sh | bashecho
eval "$(pixi completion --shell zsh)"' >> ~/.zshrc
```

2. Clone this repository to your machine:

```
git clone https://github.com/JonathanEMillar/maic_pixi.git
cd maic_pixi
```

3. Install Pixi environment:

```
pixi install
```

## Usage

1. To run MAIC, in maic_pixi/:

```
maic -f <inputfilename> -o <outputdir> -v
```

Each line of the input file describes a list of entities. The first four columns in each line specify features of the list in this line, and the fifth is a space-separated list of entity names, e.g.

`<category>` <list_label> RANKED `<unused>` entity1 entity2 entity3 ...

`<category>` <list_label> RANKED `<unused>` entity1 entity2 entity3 ...

`<category>` <list_label> UNRANKED `<unused>` entity1 entity2 entity3 ...

`<category>` <list_label> UNRANKED `<unused>` entity1 entity2 entity3 ...

## Analysis scripts

I have included a selection of downstream analysis scripts in /src. You can also use many of the functions in the [ARDSMAICr](https://github.com/baillielab/ardsmaicr) package.

## Questions

Drop me a line at <jonathan.millar@ed.ac.uk>
