# Banco de dados de teste: NSCLC-Radiomics

Esta pasta contém imagens médicas de exemplo usadas para testar os projetos deste
workspace. As imagens pertencem ao conjunto de dados público **NSCLC-Radiomics
(versão 4)**, disponibilizado pelo **The Cancer Imaging Archive (TCIA)**.

Página oficial da coleção:
[https://www.cancerimagingarchive.net/collection/nsclc-radiomics/](https://www.cancerimagingarchive.net/collection/nsclc-radiomics/)

## Conteúdo local

Os dados estão organizados em `data/`, com um diretório por paciente. Esta cópia
local contém os casos `LUNG1-001` a `LUNG1-010`, armazenados como séries DICOM.

```text
datasets/
├── README.md
└── data/
    ├── LUNG1-001/
    ├── LUNG1-002/
    ├── ...
    └── LUNG1-010/
```

O diretório `datasets` é compartilhado pelos projetos em `E:\git` e deve ser
usado como fonte central das imagens de teste. Não é necessário duplicar os
arquivos DICOM dentro de cada projeto.

Exemplo de caminho para uma série DICOM:

```text
E:\git\datasets\data\LUNG1-001\09-18-2008-StudyID-NA-69331\0.000000-NA-82046
```

## Uso

Estas imagens são destinadas a testes de carregamento DICOM, visualização,
pré-processamento, classificação, segmentação e extração de características.
Ao publicar resultados, exemplos, figuras ou métricas derivados dessas imagens,
cite o conjunto de dados original conforme a referência abaixo e consulte as
condições de uso apresentadas pelo TCIA.

## Referência

Aerts, H. J. W. L., Wee, L., Rios Velazquez, E., Leijenaar, R. T. H., Parmar,
C., Grossmann, P., Carvalho, S., Bussink, J., Monshouwer, R., Haibe-Kains, B.,
Rietveld, D., Hoebers, F., Rietbergen, M. M., Leemans, C. R., Dekker, A.,
Quackenbush, J., Gillies, R. J., & Lambin, P. (2014). *Data From
NSCLC-Radiomics* (version 4) [Data set]. The Cancer Imaging Archive.
[https://doi.org/10.7937/K9/TCIA.2015.PF0M9REI](https://doi.org/10.7937/K9/TCIA.2015.PF0M9REI)

## Citação BibTeX

```bibtex
@dataset{aerts2014nsclc_radiomics,
  author    = {Aerts, Hugo J. W. L. and Wee, Leonard and Rios Velazquez,
               Emmanuel and Leijenaar, Ralph T. H. and Parmar, Chintan and
               Grossmann, Patrick and Carvalho, Sara and Bussink, Johan and
               Monshouwer, Remco and Haibe-Kains, Benjamin and Rietveld, Daan
               and Hoebers, Frank and Rietbergen, Michiel M. and Leemans,
               C. René and Dekker, André and Quackenbush, John and Gillies,
               Robert J. and Lambin, Philippe},
  title     = {Data From NSCLC-Radiomics},
  year      = {2014},
  publisher = {The Cancer Imaging Archive},
  version   = {4},
  doi       = {10.7937/K9/TCIA.2015.PF0M9REI},
  url       = {https://doi.org/10.7937/K9/TCIA.2015.PF0M9REI}
}
```
