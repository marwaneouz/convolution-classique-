# convolution-classique-
# 🧠 Réseau de Neurones Convolutif (CNN) pour la Classification MNIST

<div align="center">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=pytorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Python-3.7%2B-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/Dataset-MNIST-red.svg" alt="MNIST">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
</div>

> **Rapport de TP** : Implémentation et comparaison de réseaux convolutifs (CNN) pour la classification des chiffres manuscrits du dataset **MNIST**, avec PyTorch.  
> 📅 **Date** : 28 août 2025  
> 👤 **Auteur** : [Ouzaina Marwane](https://github.com/marwaneouz)

---

## 📌 Objectif

Ce projet a pour but d’implémenter et comparer plusieurs architectures de réseaux de neurones convolutifs (CNN) pour la classification d’images sur le dataset **MNIST** :
- Un **CNN classique** conçu spécifiquement pour MNIST.
- **LeNet-5**, l’un des premiers CNN historiques.
- **VGG-16** et **ResNet-50**, deux architectures profondes emblématiques.

L’objectif est de comprendre les principes des CNN, d’implémenter des modèles **depuis zéro** avec PyTorch, et d’analyser comment la complexité d’un modèle influence ses performances sur une tâche simple.

---

## 🏗️ Architectures Implémentées

| Modèle | Description |
|-------|-------------|
| **CNN Classique** | Réseau simple à 3 couches convolutives + fully connected, optimisé pour MNIST. |
| **LeNet-5** | Architecture historique de Yann LeCun, idéale pour la reconnaissance de chiffres. |
| **VGG-16** | Réseau profond avec des noyaux 3x3 uniformes, implémenté from scratch. |
| **ResNet-50** | Réseau résiduel profond utilisant des *skip connections*, implémenté en PyTorch. |

> ✅ Toutes les architectures ont été implémentées **sans utiliser `torchvision.models`**.

---

## 📊 Résultats sur MNIST

| Modèle       | Précision (Test) | Perte (Test) |
|-------------|------------------|--------------|
| **LeNet-5**     | **98.90%**         | 0.0409       |
| **CNN Classique** | ~98%+           | Faible       |
| **VGG-16**      | 96.29%         | 0.1203       |
| **ResNet-50**   | 92.65%         | 0.2381       |

### 🔍 Analyse
- **LeNet-5** est le **meilleur modèle** sur MNIST, malgré sa simplicité.
- Les modèles lourds comme **ResNet-50** souffrent d’un **surapprentissage** potentiel et d’une complexité excessive pour une tâche simple.
- Un **CNN bien conçu** (comme le modèle classique) peut rivaliser avec les modèles historiques.

> ✅ **Conclusion** : *La performance ne dépend pas uniquement de la profondeur, mais de l’adéquation entre l’architecture et la tâche.*

---
 

 
