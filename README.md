# GrimoireLab Personal Utils

[GrimoireLab](http://grimoirelab.github.io) include a set of interesting tools, but sometimes I need to run specific analysis or *proof of concept ideas* not convered yet by the current platform. Usually, I need easier ways to play with projects and communities data without setting up the whole Grimoire Lab infrastructure.

This repository is my *personal playground* to test some of these ideas, mostly as [Jupyter notebooks](http://jupyter.org/).

Feel *free* to play with them!

# How to play

## Requirements

For most of the *ideas* you need:
* [Jupyter notebooks](http://jupyter.org/)
* [GrimoireLab/Perceval](https://github.com/GrimoireLab/perceval)
* [Elasticsearch](https://www.elastic.co/products/elasticsearch), [elasticsearch-py](https://github.com/elastic/elasticsearch-py) and [elasticsearch-dsl-py](https://github.com/elastic/elasticsearch-dsl-py)
* To play with generated data, you might need [Kibana](https://www.elastic.co/products/kibana)
* [utils.py](utils.py) file has some extra dependencies

There is a [settings example file](settings-example.yml) where you can define some variables to be used.

## Current *ideas*

Index generators:
* [Light Git index generator.ipynb](Light%20Git%20index%20generator.ipynb): given a list of git urls in the settings file, it generate an elasticsearch index with items showing info about commits at file level.
* [Light Meetup index generator.ipynb](Light%20Meetup%20index%20generator.ipynb): given a list of Meetup groups names in the settings file, it generate an elasticsearch index with items showing info about meetup groups *rvsps*.
* [Light Github index generator.ipynb](Light%20Github%20index%20generator.ipynb): given a list of Github repositories urls in the settings file, it generate two elasticsearch indexes called with items showing info about commits at files level, github issues and github pull requests.

Other ideas:
 * [Genderize Index.ipynb](Genderize%20Index.ipynb): given an elasticsearch index, names field in the index, an optional `names.csv` file (containing `name`, `gender`, `probability`, `count`), it update each item in the index with gender information for the indicated names field.

# Issues

Of course, there will be issues! I am not a computer scientist, and I am self-learning Python, Elasticsearch, etc. during this journey.

If you find any issue, feel free to [report it](https://github.com/jsmanrique/grimoirelab-personal-utils/issues/new).

Pull requests are also welcome, but I wouldn't recommend you losing time with this poor code. If you wanna help, [go for the real thing](http://grimoirelab.github.io)!

# What's next?

If you wanna know more about [GrimoireLab](http://grimoirelab.github.io), I recommend you to read [GrimoireLab Training](https://www.gitbook.com/book/jgbarah/grimoirelab-training/details) free and open book.

My colleague Daniel Izquierdo has been developing an interesting toolkit called [Ceres](https://github.com/dicortazar/ceres) combining [Perceval](http://github.com/grimoirelab/perceval) and [Pandas](http://pandas.pydata.org/) for data *massaging*. It's worth taking a look into [it](https://github.com/dicortazar/ceres).

# License

100% free, open source software.. of course! [MIT License](LICENSE)
