---
layout: post
title:  "Semantic segmentation : segmenter les images pour un système de conduite autonome"
date:   2022-09-10 12:00:00 +0100
categories: AI-Projects
type: "Projet IA"
image: "assets/images/portfolio/AI_08.jpg"
---

Ce projet est le 8ème des 11 projets réalisés pour valider mon diplôme d'Ingénieur IA / Data Scientist.

---
### Contexte & Objectif

Le client *(factice)* est une entreprise qui conçoit des systèmes embarqués de vision par ordinateur pour les véhicules autonomes.

Cette entreprise développe un système basé sur un pipeline en 4 parties principales:<br>

1.*ACQUISITION DES IMAGES EN TEMPS RÉEL*<br>
2.*TRAITEMENT DES IMAGES*<br>
3.*SEGMENTATION DES IMAGES*<br>
4.*SYSTÈME DE DÉCISION*

Ma mission consistait à `prendre en charge la partie segmentation` du pipeline pour transmettre des données utiles au système de décision qui vient après.

Pour ce faire, je me suis appuyé sur le jeu de données [Cityscapes](https://www.cityscapes-dataset.com/dataset-overview/) qui a l'avantage de proposer un grand nombre de photos finement annotées.

---
### GitHub
Le dépôt Git contient une présentation *(en anglais)* plus poussée du projet et du jeu de données. Par ailleurs vous y trouverez toutes les explications nécessaires pour le faire fonctionner en local.

> ##### <ico class="ti-github"></ico>&nbsp;&nbsp; <a href='https://github.com/Valkea/OC_AI_08' target='_blank'>Dépôt GitHub du projet</a>

---
### Présentation Vidéo

> ##### <a href='{{site.baseurl}}/assets/pdf/AI_P08.pdf' target='_blank'><ico><b>🗎 </b></ico>&nbsp;&nbsp;Présentation PDF associée</a>

<iframe class='youtube_video' src="https://www.youtube-nocookie.com/embed/5XJSpJ1cndw" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Note technique

> ##### <a href='{{site.baseurl}}/assets/pdf/AI_P08_Note_technique.pdf' target='_blank'>Ouvrir le document en grand</a>

{% pdf "{{site.baseurl}}/assets/pdf/AI_P08_Note_technique.pdf" no_link %}
