---
layout: post
title:  "Vehicle Recognition and Inspection System : vérifier les dommages déclarés"
date:   2023-04-05 12:00:00 +0100
categories: AI-Projects
type: "Projet IA"
image: "assets/images/portfolio/AI_MyCover.jpg"
---

Ce projet a été réalisé par une équipe internationale et pluridisciplinaire sélectionnée par Omdena. J'y ai pris part en tant qu'Ingénieur Machine Learning junior.

---
### Contexte & Objectif

Le client (MyCover) est une compagnie d'assurance automobile déjà active sur le continent africain. Pour réduire ses coûts et faciliter son travail de vérification des déclarations d'accidents, ils ont demandé à Omdena de leur fournir les bases d'un outil permettant de détecter les dommages, d'estimer leur gravité et leur coût de réparation à partir de photos ou vidéos fournies par leurs clients. Omdena a donc rassemblé une équipe de 50 personnes qui ont travaillé ensemble pendant un peu plus de 2 mois pour fournir un premier prototype.

Au sein de cette équipe, j'ai d'abord rejoint l'équipe de collecte et de préparation des données (aucune donnée n'était fournie), puis j'ai fait quelques essais de modélisation avant de finalement prendre en charge l'écriture et de l'API et le déploiement du projet dans le cloud.

Dans le groupe de collecte et de traitement des données, j'ai commencé par coder un outil personnalisé pour annoter nos données, puis j'ai aidé à collecter et à préparer les données nécessaires à un tel projet. C'était très intéressant, car jusqu'à présent, tous mes projets d'IA/ML disposaient de données (plus ou moins propres) avec lesquelles travailler... J'ai donc découvert à quel point il peut être difficile de rassembler des données `pertinentes` et à quel point une expertise en machine learning peut être nécessaire à cette toute première étape que l'on imagine à tort comme simple.

Dans le groupe de déploiement, j'ai écrit une API Flask pour inférer les dommages, leur gravités et une estimation des coûts avec les différents modèles puis j'ai déployé l'ensemble sur AWS. Dans un second temps, j'ai écrit un client de démonstration (en html5 & vanilla javascript) pour démontrer les possibilités de notre outil au client.


---
### GitHubo

Le dépôt Git contient une partie des éléménts sur lesquels j'ai été personnelement amené à travailler. Mais pour des raisons de confidentialité je ne peux pas partager l'ensemble du projet.

> ##### <ico class="ti-github"></ico>&nbsp;&nbsp; <a href='https://github.com/Valkea/Omdena_MyCover' target='_blank'>Dépôt GitHub du projet</a>

---
### Captures d'écran du projet

##### 1. Quelques vues du petit logiciel d'annotation des données

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/02.png' class='screenshots'>

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/03.png' class='screenshots'>

##### 2. Quelques vues de l'outil que nous avons utilisé pour annoter les parties abimés sur plusieurs milliers de photos

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/04.png' class='screenshots'>

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/05.png' class='screenshots'>

##### 3. Une vue simplifiée des points d'entrée de l'API

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/06.png' class='screenshots'>

##### 4. Quelques vues du client html / javascript

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/07.png' class='screenshots'>

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/08.png' class='screenshots'>

> <input type='image' src='{{site.baseurl}}/assets/images/portfolio/MyCover/09.png' class='screenshots'>

---
### Lettres de recommandations

Outre l'expérience gagnée et le plaisir de travailler sur différents aspect du projet, j'ai également eu le plaisir de recevoir deux lettres de recommandations que voici:

> ##### <a href='{{site.baseurl}}/assets/pdf/Recommendation_Letter_from_Tariq.pdf' target='_blank'><ico><b>🗎 </b></ico>&nbsp;&nbsp;Lettre de recommandation de Tariq Jamil (Senior Machine Learning Engineer)</a>

> ##### <a href='{{site.baseurl}}/assets/pdf/Recommendation_Letter_from_Vidura.pdf' target='_blank'><ico><b>🗎 </b></ico>&nbsp;&nbsp;Lettre de recommandation de Vidura Wijekoon (Product Owner & Lead ML engineer)</a>
