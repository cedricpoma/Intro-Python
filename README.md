
##<a href="http://www.insa-toulouse.fr/" ><img src="http://www.math.univ-toulouse.fr/~besse/Wikistat/Images/Logo_INSAvilletoulouse-RVB.png" style="float:left; max-width: 80px; display: inline" alt="INSA"/> |  [*Mathématiques Appliquées*](http://www.math.insa-toulouse.fr/fr/index.html), [`Science des Données`](http://www.math.insa-toulouse.fr/fr/enseignement.html) 

# <a href="https://www.python.org/"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Python_logo_and_wordmark.svg/390px-Python_logo_and_wordmark.svg.png" style="max-width: 200px; display: inline" alt="Python"/></a> pour Statistique et *Science des Données*

L'objectif de ces tutoriels, proposés sous forme de calepins ([*jupyter notebooks*](http://jupyter.org/)), est d'introduire les principaux concepts et fonctionnalités du langage [Python](https://www.python.org/) en insistant sur ceux indispensable au statisticien, maintenant *data scientist*. Syntaxe, objets et classes, fonctions graphiques, techniques de préparation (*munging* ou *wrangling*) des données, éventuellement massives (*big data*), puis leur analyse (*big data analytics*) en enchaînant phases d'[exploration](http://wikistat.fr/) et de [modélisation](http://wikistat.fr/) ou [apprentissage](http://wikistat.fr/) (machine / statistique). Des exemples plus détaillés sur des données spécifiques (en R et en python) sont proposés sur [wikistat.fr](http://wikistat.fr/) ainsi que dans les autres dépôts de ce site. Les méthodes sont exposées dans les vignettes de [wikistat](http://wikistat.fr/).

Les documents sont des calepins (*notebooks*) au format .ipynb à télécharger et ouvrir dans *Jupyter*. Il suffit pour cela de cloner le dépôt dans son propre environnement [GitHub](https://github.com/) ou de télécharger l'archive zippée.

## Tutoriels d'initiation à [Python](https://www.python.org/)
- [`Cal1-introPython`](https://github.com/wikistat/Intro-Python/blob/master/Cal1-introPython.ipynb) La syntaxe, les objects et classes de Pyhton. Initiation au langage.
- [`Cal2-PythonPandas`](https://github.com/wikistat/Intro-Python/blob/master/Cal2-PythonPandas.ipynb). Trafic de données (*data munging*) avec pandas.
- [`Cal3-PythonGraphes`](https://github.com/wikistat/Intro-Python/blob/master/Cal3-PythonGraphes.ipynb) Syntaxes de base pour des graphes en Python.
- [`Cal4-PythonProg`](https://github.com/wikistat/Intro-Python/blob/master/Cal4-PythonProg.ipynb) Programmation, classes, objets, programmation fonctionnelle.
- [`Cal5-PythonSklearnApprent`](https://github.com/wikistat/Intro-Python/blob/master/Cal5-PythonSklearnApprent.ipynb) Introduction à la modélisation Statistique et à l'apprentissage machine avec Scikit-learn; construction de *pipelines*.

## Pourquoi [Python](https://www.python.org/)

Le langage [Python](https://www.python.org/) est développé et diffusé par la [*Python Software Foundation*](https://www.python.org/psf/) selon une licence [GPL-compatible](https://docs.python.org/3/license.html). À partir d'applications initialement de calcul scientifique (image, signal...), son utilisation s'est généralisée dans de nombreux domaines et notamment pour l'analyse statistique de données pouvant être volumineuses. Il est donc "libre", efficace en calcul numérique (librairie `NumPy`), orienté objet, propose de la programmation fonctionnelle... et bénéficie d'une communauté très active qui développe de nombreuses applications et librairies. 

L'objectif de ce tutoriel est d'introduire le langage Python et quelques librairies pour préparer puis commencer à analyser des données. Lorsque celles-ci sont trop volumineuses pour la taille du disque et distribuées sur les n\oe uds d'un `cluster` sous `Hadoop` c'est encore le langage Python (API PySpark) qui permet de passer à l'échelle en utilisant la technologie [*Spark*](https://spark.apache.org/) et éventuellement la librairie [MLlib](https://spark.apache.org/mllib/). 

De façon plus précise, Python et la librairie `pandas` offrent des outils efficaces, comme le découpage automatique en morceaux (`chunks`) adaptés à la taille de la mémoire vive ou encore l'accès à des données au format binaire HDF5 (librairie `Pytable`), pour lire (format `.csv` ou fixe), gérer, pré-traiter, trafiquer (en jargon : *data munging* ou *wrangling*), visualiser des données volumineuses. Néanmoins, la parallélisation des traitements pour des très volumineuses ou en flux donc distribuées sera sans doute plus efficace avec la technologie adaptée [*Spark*](https://spark.apache.org/).

La version 3.4. de Python est celle actuellement la "plus récente". Le passage à la version 3 introduisit une [rupture de compatibilité](https://wiki.python.org/moin/Python2orPython3) par rapport à la version 2 qui est toujours en développement (2.7). Il reste actuellement nécessaire de pouvoir utiliser les 2 versions selon les librairies utilisées (la 2.7 pour Spark) et applications recherchées. La version 2.7  inclut des ajouts permettant des éléments de "rétro"-compatibilité avec la version 3. Pour l'usage rudimentaire de ces tutoriels, il semble que les deux versions soient compatibles.
