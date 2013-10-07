# pazpar2-all

This repository collects the resources and subrepositories used at SUB Göttingen to run a pazpar2 service and and use it in web sites.

2012-2013 Sven-S. Porst, [SUB Göttingen](http://www.sub.uni-goettingen.de) <porst@sub.uni-goettingen.de>


## Subfolders

* __[settings-SUB](https://github.com/subugoe/pazpar2-SUB)__ – pazpar2 settings used or tested at SUB Göttingen. In addition to the configuration files, this repository includes as submodules:
	* Index Data’s [pazpar2](https://github.com/subugoe/pazpar2) and [yaz](http://git.indexdata.com/?p=yaz.git) software
	* the [pazpar2-etc](https://github.com/subugoe/pazpar2-etc) repository.
* __[typo3-pazpar2](https://github.com/subugoe/typo3-pazpar2)__ – A TYPO3 extension to include pazpar2 as a content element in a TYPO3 site. The extension is named »pazpar2« and is also available from TER for comfortable installation via TYPO3’s extension manager.
	* The JavaScript display code is provided by [pazpar2-js-client](https://github.com/subugoe/pazpar2-js-client) which is included as a submodule.
* [pazpar2](https://github.com/subugoe/pazpar2) – [Index Data](http://www.indexdata.com/)’s pazpar2 with small patches.
* [pazpar2-etc](https://github.com/subugoe/pazpar2-etc) – updated versions of files in pazpar/etc (having those in a separate repository lets us use Index Data’s »pure« pazpar2 repository without having to worry about merging issues).
* [pazpar2-access](https://github.com/subugoe/pazpar2-access) – a simple PHP script to moderate access to pazpar2’s init and settings commands: used to control access based on the user’s IP address based on a service by GBV.
* [opac-2-atom](https://github.com/subugoe/opac-2-atom) – submodule with a simple script to convert Pica Opac XML output to an Atom feed. Used for feed subscriptions created by the pazpar2-neuerwerbungen TYPO3 Plug-In. Probably not interesting for external users.
* [pazpar2-js-client](https://github.com/subugoe/pazpar2-js-client) – JavaScript client to communicate with pazpar2 and display the results. This includes:
	* the flot graphing libary,
	* scripts and XSL to convert from pazpar2’s internal metadata format to RIS and BibTeX.
	* Media icons are provided by [sub-iconfont](https://github.com/subugoe/sub-iconfont) which is included as a submodule.
* [sub-iconfont](https://github.com/subugoe/sub-iconfont) – icon font for media types.




## Example Sites

This setup and code is used in various SUB Göttingen web sites:

* [Library of Anglo-American Culture](http://aac.sub.uni-goettingen.de) uses pazpar2 in various places:
	* for the metasearch on the [main page](http://aac.sub.uni-goettingen.de/)
	* for [new acquisitions](http://aac.sub.uni-goettingen.de/en/new/) – uses the pazpar2-neuerwerbungen Plug-In of the pazpar2 TYPO3 extension, subject selection is based on data provided by the [nkwgok TYPO3-extension](http://aac.sub.uni-goettingen.de/en/new/)
	* for the [subject search](http://aac.sub.uni-goettingen.de/en/literature/subjects/) – subject selection is driven by the [nkwgok TYPO3-extension](https://github.com/subugoe/typo3-nkwgok) for displaying subject hierarchies
* [GEO-LEO](http://geo-leo.de) likewise:
	* for the metasearch on the [main page](http://geo-leo.de)
	* for the [subject search](http://geo-leo.de/themen/)
* [vifamath](http://geo-leo.de) likewise:
	* for the metasearch on the [main page](http://vifamath.de)
	* for the [subject search](http://vifamath.de/subject-catalogue/?L=1)
* [SUB Göttingen homepage](http://www.sub.uni-goettingen.de):
	* [Metasearch Page for additional catalogues](http://www.sub.uni-goettingen.de/en/search/articles-and-full-texts/)
	* New acquisitions pages, e.g. [Mathematics](http://www.sub.uni-goettingen.de/en/subjects/subject-areas-natural-sciences-mathematics-and-computer-science/mathematics/neuerwerbungen/)
