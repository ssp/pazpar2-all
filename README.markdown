# pazpar2-all

This repository collects the resources and subrepositories used at SUB Göttingen to run a pazpar2 service and and use it in web sites.

2012 Sven-S. Porst, [SUB Göttingen](http://www.sub.uni-goettingen.de) <porst@sub.uni-goettingen.de>


## Subfolders

* [opac-2-atom](https://github.com/ssp/opac-2-atom) – submodule with a simple script to convert Pica Opac XML output to an Atom feed. Used for feed subscriptions created by the pazpar2-neuerwerbungen TYPO3 Plug-In. Probably not interesting for external users.
* [pazpar2](http://git.indexdata.com/?p=pazpar2.git) – [Index Data](http://www.indexdata.com/)’s original pazpar2 repository.
* [pazpar2-access](http://git.indexdata.com/?p=pazpar2.git) – a simple PHP script to moderate access to pazpar2’s init and settings commands: used to control access based on the user’s IP address based on a service by GBV.
* [pazpar2-etc](https://github.com/ssp/pazpar2-etc) – updated versions of files in pazpar/etc (having those in a separate repository lets us use Indexdata’s »pure« pazpar2 repository without having to worry about merging issues).
* [pazpar2-js-client](https://github.com/ssp/pazpar2-js-client) – JavaScript client to communicate with pazpar2 and display the results. This includes:
	* the flot graphing libary,
	* scripts and XSL to convert from pazpar2’s internal metadata format to RIS and BibTeX.
* [settings-SUB](https://github.com/ssp/pazpar2-SUB) – pazpar2 settings used or tested at SUB Göttingen. This repository includes as submodules:
	* Index Data’s [pazpar2](http://git.indexdata.com/?p=pazpar2.git) and [yaz](http://git.indexdata.com/?p=yaz.git) repositories,
	* the [pazpar2-etc](https://github.com/ssp/pazpar2-etc) repository.
* [typo3-pazpar2](https://github.com/ssp/typo3-pazpar2): A TYPO3 extension to include pazpar2 as a content element in a TYPO3 site. The extension is named »pazpar2« and is also available from TER for comfortable installation via TYPO3’s extension manager.
	* The JavaScript display code is provided by  [pazpar2-js-client](https://github.com/ssp/pazpar2-js-client) which is included as a submodule.




## Example Sites

You can find this code in use in various SUB Göttingen web sites:

* [Library of Anglo-American Culture](http://aac.sub.uni-goettingen.de) Uses pazpar2 in various places:
	* for the metasearch on the [main page](http://aac.sub.uni-goettingen.de/)
	* for [new acquisitions](http://aac.sub.uni-goettingen.de/en/new/) – uses the pazpar2-neuerwerbungen Plug-In of the pazpar2 TYPO3 extension, subject selection is based on data provided by the [nkwgok TYPO3-extension](http://aac.sub.uni-goettingen.de/en/new/)
	* for the [subject search](http://aac.sub.uni-goettingen.de/en/literature/subjects/) – subject selection is driven by the [nkwgok TYPO3-extension](http://aac.sub.uni-goettingen.de/en/new/) for displaying subject hierarchies
* [SUB Göttingen homepage](http://www.sub.uni-goettingen.de):
	* [Metasearch Page for additional catalogues]()http://www.sub.uni-goettingen.de/suche/aufsaetze-und-elektronische-volltexte/)
	* New acquisitions pages, e.g. [Mathematics](http://www.sub.uni-goettingen.de/faecher-naturwissenschaften-mathematik-und-informatik/mathematik/neuerwerbungen/) – uses the pazpar2-neuerwerbungen Plug-In of the pazpar2 TYPO3 extension, subject selection is based on data provided by the [nkwgok TYPO3-extension](http://aac.sub.uni-goettingen.de/en/new/)

