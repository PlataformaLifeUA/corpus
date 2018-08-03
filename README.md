# Corpus
This repository contains the files composing the life! gold standard corpus and further improvements. It has been created by [PlataformaLifeUA](https://gplsi.dlsi.ua.es/life/).

Files are stored as XML following Gate standoff format. The root element of each file is ```<GateDocument>```. Every document contains:
- ```<TextWithNodes>``` to store the text of the annotated document.  ```<Node>``` indicates that this position is either the initial and final character offset of an annotation. 
- For files which belong to gold standard corpus, annotations are organised in several ```<AnnotationSet>```. Each set includes detailed anotations carried out by different authors. Specifically:
	- ```15 markups``` and ```80 markups``` contains manual annotations performed by human raters (with identifiers 15 and 80).
	- ```consensus markups``` gathers the gold standard annotations that were included by consensus of the Life Platform team.
	- ```LingPipe markups``` includes annotations included by the tokenizer and sentence splitter from LingPipe pluging.

## Statistics
At this moment, Life! corpus contains 8043 tokens and 536 sentences in 102 document. Each document is a message extracted from Surface or Deep Web Social Networks. Each message contains three properties manually annotated, namely: Language, Alert level and Type of message. 

Next tables provide more details of each property:

| Language | Quantity of messages |
|----------|----------------------|
| English  | 71                   |
| Spanish  | 31                   |


| Alert Level | Quantity | English | Spanish |
|-------------|----------|---------|---------|
| No risk     | 70       |   45    | 25      |
| Urgent      | 19 		 |   15	   | 4 		 |
| Possible    | 8 		 |   6	   | 2		 |
| Immediate   | 5 		 |	 5 	   | 0		 |


| Type of message 		| Quantity | English | Spanish |
|-----------------------|----------|---------|---------|
| Undefined        		| 38 	   | 32 	 | 6 	   |
| Auto-Pro-Suicide      | 22 	   | 20 	 | 2 	   |
| Sadness or melancholy | 11 	   | 1 		 | 10 	   |
| Auto-No-Pro-Suicide   | 10 	   | 7 		 | 3	   |
| Depression   			| 9  	   | 5 		 | 4 	   |
| Suicide curiosity		| 5 + 1    | 3 + 1   | 2 	   |
| Irony                 | 3  	   | 2       | 1       |
| Citation              | 2  	   | 0       | 2       |
| Mysticism             | 1  	   | 0       | 1       |
| Instigator            | 1  	   | 1       | 0       |


## Built with
- [Gate Developer 8.2](https://gate.ac.uk/): The annotation tool used

## Sponsors
This resource is the output of the following research projects: (i) Análisis de Sentimientos Aplicado a la Prevención del Suicidio en las Redes Sociales (ASAP) funded by Fundación BBVA, (ii) Representación canónica y transformaciones de los textos aplicado a las Tecnologías del Lenguaje Humano (RESCATA - Ref. TIN2015-65100-R) and (iii) Reconocimiento de Entidades Digitales: Enriquecimiento y Seguimiento (REDES - Ref. TIN2015-65136-C2-2-R)