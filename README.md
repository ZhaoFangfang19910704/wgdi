# WGDI

![Latest PyPI version](https://img.shields.io/pypi/v/wgdi.svg) [![Downloads](https://pepy.tech/badge/wgdi/month)](https://pepy.tech/project/wgdi) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/wgdi/README.html)

| | |
| --- | --- |
| Author  | Pengchuan Sun ([sunpengchuan](https//github.com/sunpengchuan)) |
| Email   | <sunpengchuan@gmail.com> |
| License | [BSD](http://creativecommons.org/licenses/BSD/) |

## Description

WGDI (Whole-Genome Duplication Integrated analysis), a Python-based command-line tool that facilitates comprehensive analysis of recursive polyploidizations and cross-species genome alignments.

WGDI supports three main workflows (polyploid inference, hierarchical inference of genomic homology, and ancestral chromosomal karyotyping) that can improve detection of WGD and characterization of related events. It incorporates a more sensitive and accurate collinearity detection algorithm than previous softwares, and can accelerate WGD-related karyotype research.

## Installation

Python package and command line interface (IDLE) for the analysis of whole genome duplications (WGDI). WGDI can be deployed in Windows, Linux, and Mac OS operating systems and can be installed via pip and conda.

#### Bioconda

```
conda install -c bioconda  wgdi
```

#### Pypi

```
pip3 install wgdi
```

Documentation for installation along with a user tutorial, a default parameter file, and test data are provided. please consult the docs at <http://wgdi.readthedocs.io/en/latest/>.

## Tips

Here are some videos with simple examples of WGDI.

###### [WGDI的简单使用（一）](https://www.bilibili.com/video/BV1qK4y1U7eK) or https://youtu.be/k-S6FVcBIQw

###### [WGDI的简单使用（二）](https://www.bilibili.com/video/BV195411P7L1) or https://youtu.be/QiZYFYGclyE

chatting group QQ : 966612552

## Citating WGDI

If you use wgdi in your work, please cite:

> Sun P., Jiao B., Yang Y., Shan L., Li T., Li X., Xi Z., Wang X., and Liu J. (2022). WGDI: A user-friendly toolkit for evolutionary analyses of whole-genome duplications and ancestral karyotypes. Mol. Plant. doi: https://doi.org/10.1016/j.molp.2022.10.018.

## News

## 0.6.2
* Added find shared fusions between species (-sf).

## 0.6.1

* Fixed issue with alignment (-a). Only version 0.6.0 has this bug.

## 0.6.0

* Fixed issue with improved collinearity (-icl).
* Added a parameter 'tandem_ratio' to blockinfo (-bi).

## 0.5.9

* Update the improved collinearity (-icl). Faster than before, but lower than MCscanX, JCVI.
* Fixed issue with ancestral karyotype repertoire (-akr).

## 0.5.8

* Fixed issue with gene names (-ks).

## 0.5.7
- Fixed issue with chromosome order (-ak).
- Fixed issue with gene names (-ks).  This version is not fixed, please install the latest version.

## 0.5.5 and 0.5.6
* Add ancestral karyotype (-ak)
* Add ancestral karyotype repertoire (-akr)

## 0.5.4
* Improved the alignmenttrees (-km) effect.
* little change (-at).

## 0.5.3
* Fixed legend issue with (-kf).
* Fixed calculate Ks issue with (-ks).
* Improved the karyotype_mapping (-km) effect.
* Improved the alignmenttrees (-at) effect.

## 0.5.2
* Fixed some bugs.

## 0.5.1
* Fixed the error of the command (-conf).
* Improved the karyotype_mapping (-km) effect.
* Added the available data set of alignmenttree (-at). Low copy data set (for example, single-copy_groups.tsv of sonicparanoid2 software).

## 0.4.9
* The latest version adds karyotype_mapping (-km) and karyotype (-k) display.
* The latest version changes the calculation of extracting pvalue from collinearity (-icl), making this parameter more sensitive. Therefore, it is recommended to set to 0.2 instead of 0.05.
* The latest version has also changed the drawing display of ksfigure (-kf) to make it more beautiful.
