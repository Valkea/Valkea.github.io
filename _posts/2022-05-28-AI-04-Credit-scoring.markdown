---
layout: post
title:  "Credit-scoring : aide à la décision pour des micro-prêts"
date:   2022-05-28 12:00:00 +0100
categories: AI-Projects
type: "Projet IA"
image: "assets/images/portfolio/AI_04.jpg"
---

Ce projet est le 4ème des 11 projets réalisés pour valider mon diplôme d'Ingénieur IA / Data Scientist.

---
### Contexte & Objectif

Le client *(factice)* est une startup qui propose des crédits à la consommation pour des personnes ayant peu ou pas d'historique de prêt. Son intérêt est de prêter aux clients qui seront en capacité de rembourser pour faire du chiffre, mais aussi d'éviter de prêter à ceux qui ne le pourront pas pour éviter de les mettre en difficulté financière ou de faire perdre de l'argent à l'entreprise.

Il a donc été décidé de développer un modèle de crédit-scoring, mais avec une forte contrainte d'intérpretabilité des résultats. En effet, en cas de refus, le RGPD stipule qu'il faut pouvoir expliquer simplement la décision prise par un système automatisé. Il convenait donc de fournir aux chargés de clientèle le moyen d'expliquer les motivations de l'algorithme pour que le client sache ce qu'il doit éventuellement améliorer. Mais c'est également nécessaire pour motiver l'accord d'un prêt auprès de la direction de la banque.

Ma mission était de `fournir un outil d'évaluation et de classification des demandes de crédits`, qui calcule donc la probabilité qu’un client le rembourse, puis classifie la demande en *accordé* ou *refusé*. Mais je devais également `utiliser un algorithme qui puisse être interprété` tant localement *(pour expliquer un cas précis)* que globalement *(pour vérifier la cohérence avec les connaissances métiers)*.

---
### GitHub
Le dépôt Git contient une présentation *(en anglais)* plus poussée du projet et du jeu de données. Par ailleurs vous y trouverez toutes les explications nécessaires pour le faire fonctionner en local.

> ##### <ico class="ti-github"></ico>&nbsp;&nbsp; <a href='https://github.com/Valkea/OC_AI_04' target='_blank'>Dépôt GitHub du projet</a>

---
### Présentation Vidéo

> ##### <a href='{{site.baseurl}}/assets/pdf/AI_P04.pdf' target='_blank'><ico><b>🗎 </b></ico>&nbsp;&nbsp;Présentation PDF associée</a>

<iframe class='youtube_video' src="https://www.youtube-nocookie.com/embed/EtK3HNdhMgc" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
