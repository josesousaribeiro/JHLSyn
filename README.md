# JHLSyn

HLSyn speech synthesizer developed in JAVA.

The HLSyn can then be used to generate the input file of the KLSYN88, having the 48 necessary parameters to  perform speech synthesis with Klatt. 

Generally speaking, HLSyn is a “high-level” synthesizer that expands its 13 input parameters into the 48 parameters of the “low-level” KLSYN88 synthesizer.

Both HLSyn and Klatt are well known in the field of speech synthesis, especially as part of solutions to human speech imitation problems.

JHLSyn was developed based on its previous implementation (made in C language) and seeks to be an alternative to voice imitation systems that are based on JAVA.


# Autor of software:

José Ribeiro - site: https://sites.google.com/view/jose-sousa-ribeiro

# Tutorial:

Example of HLSyn file necessary to run the synthesize:


AG AL AB AN UE F0 F1 F2 F3 F4 PS DC AP

100 1000 1000 0 0 1105 489 1650 2502 3500 200 0 0

100 1000 1000 0 0 1114 489 1650 2502 3500 200 0 0

250 1000 1000 0 0 1125 489 1650 2502 3500 350 0 0

328 1000 1000 0 0 1130 489 1650 2502 3500 500 0 0

368 1000 1000 0 0 1136 489 1650 2502 3500 650 0 0

390 1000 1000 0 0 1144 489 1650 2502 3500 800 0 0

402 1000 1000 0 0 1155 489 1650 2502 3500 950 0 0

410 1000 1000 0 0 1166 489 1650 2502 3500 960 0 0

415 1000 1000 0 0 1177 489 1650 2502 3500 970 0 0

419 1000 1000 0 0 1190 489 1650 2502 3500 972 0 0

423 1000 1000 0 0 1200 489 1650 2502 3500 964 0 0

426 1000 1000 0 0 1212 489 1650 2502 3500 956 0 0

429 1000 1000 0 0 1223 489 1650 2502 3500 948 0 0

...

432 1000 1000 0 0 1234 489 1650 2502 3500 940 0 0

2158 1000 1000 0 0 1079 494 1508 1808 3500 0 0 0

2158 1000 1000 0 0 1075 494 1508 1808 3500 0 0 0

2158 1000 1000 0 0 1072 495 1509 1809 3500 0 0 0

```

To run JHLSyn just run the command below in the directory where the .jar is located.

```java
java -jar JHLsyn.jar ./hldata2.hlsyn
```

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

Obs1: O arquivo 'hldata2.hlsyn' contém todos os parâmetros do HLSyn.

Obs2: A saída é um arquivo .raw referente ao áudio sintetizado.

Obs3: O arquivo JHLSyn.zip é o projeto java da IDE eclipse utilizado no desenvolvimento.

Esta ferramenta foi desenvolvida durante a pesquisa do artigo: Utterance copy for Klatt's speech synthesizer using genetic algorithm.

# Cite nosso artigo:

```
@inproceedings{sousa2014utterance,
  title={Utterance copy for Klatt's speech synthesizer using genetic algorithm},
  author={Sousa, Jos{\'e} and Ara{\'u}jo, Fab{\'\i}ola and Klautau, Aldebaro},
  booktitle={2014 IEEE Spoken Language Technology Workshop (SLT)},
  pages={89--94},
  year={2014},
  organization={IEEE}
}


