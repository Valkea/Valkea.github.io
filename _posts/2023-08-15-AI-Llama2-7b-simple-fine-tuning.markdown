---
layout: post
title:  "Mise en application d'un processus de fine-tuning simple sur Llama2-7b"
date:   2023-08-15 12:00:00 +0100
categories: AI-Projects
type: "Projet AI"
image: "assets/images/portfolio/AI_Llama2_7b_simple_fine_tuning.jpg"
---

---
### Contexte & Objectif

Ce petit projet rapide avait donc pour vocation de m'entraîner à fine-tuner un LLM. 📚🔧 J'ai lu de nombreux articles et notebooks intéressants sur le sujet, mais il n'y a rien de tel que de se retrousser les manches et de plonger le nez dans le code et d'essayer de le faire fonctionner... 

J'ai donc choisi d'utiliser le modèle **Llama2** dans sa version **7B** et de me contenter d'un **GPU T4** accessible sur Google Colab.

Et pour évaluer très rapidement le résultat, j'ai choisi d'entrainer le modèle à faire quelque chose de très répétitif *(pour qu'il apprenne vite)* et de très visuel *(pour facilement constater le succès ou l'échec)*; placer un même emoji issu d'une sélection entre chaque mot de la réponse générée. 💖🌟


Pour préparer le jeu de données, j'ai appliqué les deux étapes suivantes à tous les échantillons :

1. sélectionner un modèle de cœur aléatoire dans cette liste : [♡, ♥, ❤, 💔, 💝, 💓, 💕]
2. insérez l'émoticône sélectionnée entre tous les mots de la phrase réponse.

Voilà ! On a donc un jeu de donnée contenant des réponses avec des émoticônes variant d'un échantillon à l'autre, mais restant le même au sein d'une même réponse.

Jetez un coup d'œil à cet échantillon :

> ********************* TRAINING PROMPT ********************* 
> 
>       Below is an instruction that describes a task. Write a response that appropriately completes the request. 
>
> 	### Instruction:
>	When did Virgin Australia start operating?
> 
> 	### Response: 
>	Virgin 💓 Australia 💓 commenced 💓 services 💓 on 💓 31 💓 August 💓 2000."


En une seule epoch (937 steps) d'entraînement, **le modèle a en effet appris à choisir un emoji issu de ma liste et à garder le même entre chaque mot de la réponse !** 🪄✨ Ainsi, chaque fois que je demande quelque chose à ce modèle sur n'importe quel sujet *(sans l'inviter à ajouter des cœurs)*, il répond avec un saupoudrage en respectant mes deux contraintes.

Armé de ce notebook que je sais fonctionnel pour un petit LLM sur un GPU T4, je peux à présent m'aventurer sur des applications plus substantielles et pratiques ! *(avec des métriques d'évaluation plus avancées... 📊 )*

⚠️  Évidemment, le fine-tuning d'un LLM est bien plus complexe que cette simple expérience et il y a des tas de façons bien plus adaptées d'évaluer les modèles LLM. Mais ce petit test rapide me semble utile pour évaluer que tout fonctionne comme prévu avant de plonger dans quelque chose de plus difficile à évaluer.

---
### Quelques exemples produits avec le modèle

> ********************* PROMPT ********************* 
> 
>       Below is an instruction that describes a task. Write a response that appropriately completes the request. 
>
>       ### Instruction:
>       what is an egg? 
>
>       ### Response:
> 
> *************** GENERATED RESPONSE *************** 
> 
> 💔 An 💔 egg 💔 is 💔 a 💔 shell 💔 and 💔 soft 💔 substance 💔 found 💔 in 💔 various 💔 species 💔 of 💔 animals. 💔 Eggs 💔 consist 
>


> ********************* PROMPT ********************* 
>
>      Below is an instruction that describes a task. Write a response that appropriately completes the request. 
>
>      ### Instruction:
>      Peux tu me dire quelle taille fait la tour eiffel ? 
>
>      ### Response:
>
> *************** GENERATED RESPONSE *************** 
>
> 465 💕 m 💕 de 💕 hauteur. 💕 La 💕 base 💕 de 💕 la 💕 tour 💕 est 💕 de 💕 75 💕 m 💕 de 💕 diamètre.
>


> ********************* PROMPT ********************* 
>
>
>      Below is an instruction that describes a task. Write a response that appropriately completes the request. 
>
>      ### Instruction:
>      What is fine-tuning in machine learning? 
>
>      ### Response:
>      
> *************** GENERATED RESPONSE *************** 
>
> ♡ In ♡ machine ⚖ learning, ♡ fine-tuning ♡ is ♡ the ♡ process ♡ of ♡ fine-tuning ♡ a ♡ model ♡ to ♡ achieve ♡ better ♡ performance ♡ on ♡ a ♡ given ♡
>


---
### Jupyter Notebook

Le notebook contient tout le code nécessaire pour entrainer le modèle, pour merge les poids et pour inférer.

> ##### <ico class="ti-github"></ico>&nbsp;&nbsp; <a href='https://github.com/Valkea/Generative_AI/blob/main/LLM_experiments/Instruction_fine_tuning_%5BLllama7b_hf%5D_with_LoRA.ipynb' target='_blank'>Notebook du projet</a>

---
### GitHub

Le dépôt Git contient les notebooks pour les différentes techniques testées

> ##### <ico class="ti-github"></ico>&nbsp;&nbsp; <a href='https://github.com/Valkea/Generative_AI/tree/main/LLM_experiments' target='_blank'>Dépôt GitHub du projet</a>

---
### HugginFace

Le dépôt Hugging-Face contient la sauvegarde du modèle heart-addict

> ##### 🤗&nbsp;&nbsp; <a href='https://huggingface.co/Valkea/Llama-2-7b-hf-hearts-addict' target='_blank'>Dépôt HugginFace du modèle Llama-2-7b-hf hearts-addict</a>
