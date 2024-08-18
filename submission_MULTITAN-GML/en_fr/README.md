<p align="center">


  <p align="center">
    Team MULTITAN-GML : systems description
  </p>
</p>


## Table of contents

- [Participants](#participants)
- [What's included](#whats-included)
- [Systems](#systems)
- [Copyright and license](#copyright-and-license)


## Participants

Team members

- Lichao Zhu, CLILLAC-ARP, Université Paris Cité, <lichao.zhu@u-paris.fr>
- Maria Zimmina-Poirot, CLILLAC-ARP, Université Paris Cité, <maria.zimina-poirot@u-paris.fr>
- Behnoosh Namdar, CLILLAC-ARP, Université Paris Cité, <behnooshnamdar@gmail.com>
- Nicolas Ballier, CLILLAC-ARP, Université Paris Cité, <nicolas.ballier@u-paris.fr>


## What's included

```
submission_MULTITAN-GML/
└── en_fr/
    ├── system-1.txt
    ├── system-2.txt
    ├── system-3.txt
    ├── README.md

```

## Systems

The first two systems are of *transformer* architecture. 

1. (primary) Model Studio Lite (Systran, under commercial license) "Dialog" Specialized engine: the system is fine-tuned with 2022 Chat Task (train, valid, test) and 2024 Chat Task (valid) data on a "Dialog" in-domain specialized model. We have used 13,622 aligned en-fr segments (122,905 words in English and 127,335 words in French). The translation output is post-edited by ChatGPT4o by prompt;
2. (contrastive) NLLB 3.3B baseline (CC-BY-NC license): due to technical problems, we cannot fine-tune Nllb 3.3B baseline model. We have produced translations from scrtach by using Nllb baseline model. The output is also post-edited by ChatGPT4o by prompt;
3. (contrastive) Deep_translator baseline (MIT license): we have used Deep_translator API to translate the testset and then have the output post-edited by ChatGPT4o. 

## Copyright and license

- Model Studio Lite : Systran (under commercial license), [https://modelstudio-lite.systran.net](https://modelstudio-lite.systran.net)
- NLLB 3.3B baseline : CC-BY-NC license, [https://github.com/facebookresearch/fairseq/tree/nllb/examples/nllb](https://github.com/facebookresearch/fairseq/tree/nllb/examples/nllb)
- Deep-translator baseline : MIT license, [https://pypi.org/project/deep-translator/](https://pypi.org/project/deep-translator/)
