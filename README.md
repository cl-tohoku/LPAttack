# LPAttack: A Feasible Annotation Scheme for Capturing Logic Pattern of Attacks in Arguments

## Overview
LPAttack (Logic Pattern of Attack) is an annotation scheme that captures the common modes and complex rhetorical moves in attacks in arguments along with the implicit presuppositions and value judgments. This repository consists the corpus (logic patterns of attacks of 250 debates) annotated by the LPAttack scheme and the annotation guidelines.

![overview](https://github.com/cl-tohoku/LPAttack/blob/master/lpattack_example.jpg "overview")

## Corpus
We utilized the debates from the TYPIC dataset (Naito et al. 2022) for LPAttack annotation. Each debate consists an Initial argument, referred to as "PM Speech" (speech from Prime Minister) and a Counterargument, referred to as "LO Speech" (speech from Leader of Opposition). The debates are wriiten for 2 topics: `Death penalty should be abolished` and `Homework should be abolished`. 

In each of the topic folder, the `JSON` folder consists the data the `DRAWIO` folder consists the visual diagrams for the data (can be opened and seen using https://www.diagrams.net/).

## Citation
If you use the data in your research, please cite the following paper.
```
@InProceedings{mim-EtAl:2022:LREC,
  author    = {Mim, Farjana Sultana and Inoue, Naoya and Naito, Shoichi and Singh, Keshav and Inui, Kentaro},
  title     = {LPAttack: A Feasible Annotation Scheme for Capturing Logic Pattern of Attacks in Arguments},
  booktitle      = {Proceedings of the Language Resources and Evaluation Conference},
  year           = {2022},
  publisher      = {European Language Resources Association},
  pages     = {2446–2459},
  url       = {http://www.lrec-conf.org/proceedings/lrec2022/pdf/2022.lrec-1.261.pdf}
}
```

 
