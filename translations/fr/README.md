<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "18318279bb851dc2c709bfc6a26f6e1d",
  "translation_date": "2025-05-07T14:04:40+00:00",
  "source_file": "README.md",
  "language_code": "fr"
}
-->
![Logo](../../imgs/logo.png)

# Co-op Translator : Automatisez facilement la traduction de votre documentation éducative

_Automatisez simplement la traduction de votre documentation en plusieurs langues pour toucher un public mondial._

[![Python package](https://img.shields.io/pypi/v/co-op-translator?color=4BA3FF)](https://pypi.org/project/co-op-translator/)
[![License: MIT](https://img.shields.io/github/license/azure/co-op-translator?color=4BA3FF)](https://github.com/azure/co-op-translator/blob/main/LICENSE)
[![Downloads](https://static.pepy.tech/badge/co-op-translator)](https://pepy.tech/project/co-op-translator)
[![Downloads](https://static.pepy.tech/badge/co-op-translator/month)](https://pepy.tech/project/co-op-translator)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

[![GitHub contributors](https://img.shields.io/github/contributors/azure/co-op-translator.svg)](https://GitHub.com/azure/co-op-translator/graphs/contributors/)
[![GitHub issues](https://img.shields.io/github/issues/azure/co-op-translator.svg)](https://GitHub.com/azure/co-op-translator/issues/)
[![GitHub pull-requests](https://img.shields.io/github/issues-pr/azure/co-op-translator.svg)](https://GitHub.com/azure/co-op-translator/pulls/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

### Support linguistique assuré par Co-op Translator

[Korean](../ko/README.md) | [Japanese](../ja/README.md) | [Chinese (Simplified)](../zh/README.md) | [Chinese (Traditional, Taiwan)](../tw/README.md) | [Spanish](../es/README.md) | [French](./README.md) | [German](../de/README.md) | [Portuguese (Brazil)](../br/README.md) | [Hindi](../hi/README.md) | [Russian](../ru/README.md) | [Turkish](../tr/README.md) | [Arabic](../ar/README.md) | [Indonesian](../id/README.md) | [Vietnamese](../vi/README.md)

[![GitHub watchers](https://img.shields.io/github/watchers/azure/co-op-translator.svg?style=social&label=Watch)](https://GitHub.com/azure/co-op-translator/watchers/)
[![GitHub forks](https://img.shields.io/github/forks/azure/co-op-translator.svg?style=social&label=Fork)](https://GitHub.com/azure/co-op-translator/network/)
[![GitHub stars](https://img.shields.io/github/stars/azure/co-op-translator.svg?style=social&label=Star)](https://GitHub.com/azure/co-op-translator/stargazers/)

[![Azure AI Community Discord](https://dcbadge.vercel.app/api/server/ByRwuEEgH4)](https://discord.com/invite/ByRwuEEgH4)

[![Open in GitHub Codespaces](https://img.shields.io/static/v1?style=for-the-badge&label=Github%20Codespaces&message=Open&color=24292F&logo=github)](https://codespaces.new/azure/co-op-translator)
[![Open in Dev Containers](https://img.shields.io/static/v1?style=for-the-badge&label=VS%20Code%20Dev%20Containers&message=Open&color=007ACC&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/azure/co-op-translator)

> [!TIP]
> **Automatisation Puissante** : Maintenant avec le support de GitHub Actions ! Traduisez automatiquement votre documentation dès qu’une modification est apportée à votre dépôt, en gardant tout à jour sans effort. [En savoir plus](../..).

## Modèles et Services Supportés

| Type                  | Nom                           |
|-----------------------|--------------------------------|
| Language Model        | ![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-blue?style=flat-square) ![OpenAI](https://img.shields.io/badge/OpenAI-green?style=flat-square&logo=openai) |
| Computer Vision       | ![Azure Computer Vision](https://img.shields.io/badge/Azure_Computer_Vision-blue?style=flat-square) |

> [!NOTE]
> Si un service de vision par ordinateur n’est pas disponible, le co-op translator basculera en [mode Markdown uniquement](./getting_started/markdown-only-mode.md).

## Aperçu : Simplifiez la Traduction de Vos Contenus Éducatifs

Les barrières linguistiques limitent fortement l’accès aux ressources éducatives précieuses et aux connaissances techniques pour les apprenants et développeurs du monde entier. Cela restreint la participation et ralentit le rythme de l’innovation et de l’apprentissage à l’échelle globale.

**Co-op Translator** est né du besoin de résoudre le processus inefficace de traduction manuelle pour les grandes séries éducatives de Microsoft (comme les guides « Pour les débutants »). Il est devenu un outil puissant et facile à utiliser, conçu pour abattre ces barrières pour tous. En fournissant des traductions automatisées de haute qualité via CLI et GitHub Actions, Co-op Translator permet aux enseignants, étudiants, chercheurs et développeurs du monde entier de partager et d’accéder au savoir sans contraintes linguistiques.

Découvrez comment Co-op Translator organise le contenu éducatif traduit :

![Example](../../imgs/translation-ex.png)

Les fichiers Markdown et les textes des images sont automatiquement traduits et soigneusement organisés dans des dossiers spécifiques à chaque langue.

**Offrez dès aujourd’hui un accès mondial à vos contenus éducatifs grâce à Co-op Translator !**

## Soutenir l’Accès Global aux Ressources d’Apprentissage de Microsoft

Co-op Translator aide à combler le fossé linguistique pour les initiatives éducatives clés de Microsoft, en automatisant la traduction des dépôts qui servent une communauté mondiale de développeurs. Voici quelques exemples utilisant actuellement Co-op Translator :

[![ML-For-Beginners](https://github-readme-stats.vercel.app/api/pin/?username=microsoft&repo=ML-For-Beginners&bg_color=ffffff&title_color=0078D4&text_color=333333&border_color=c0d8f0&border_radius=10)](https://github.com/microsoft/ML-For-Beginners)
[![Generative-AI-for-beginners-dotnet](https://github-readme-stats.vercel.app/api/pin/?username=microsoft&repo=Generative-AI-for-beginners-dotnet&bg_color=ffffff&title_color=0078D4&text_color=333333&border_color=c0d8f0&border_radius=10)](https://github.com/microsoft/Generative-AI-for-beginners-dotnet)
[![AI-For-Beginners](https://github-readme-stats.vercel.app/api/pin/?username=microsoft&repo=AI-For-Beginners&bg_color=ffffff&title_color=0078D4&text_color=333333&border_color=c0d8f0&border_radius=10)](https://github.com/microsoft/AI-For-Beginners)
[![ai-agents-for-beginners](https://github-readme-stats.vercel.app/api/pin/?username=microsoft&repo=ai-agents-for-beginners&bg_color=ffffff&title_color=0078D4&text_color=333333&border_color=c0d8f0&border_radius=10)](https://github.com/microsoft/ai-agents-for-beginners)
[![PhiCookBook](https://github-readme-stats.vercel.app/api/pin/?username=microsoft&repo=PhiCookBook&bg_color=ffffff&title_color=0078D4&text_color=333333&border_color=c0d8f0&border_radius=10)](https://github.com/microsoft/PhiCookBook)

## Fonctionnalités Clés

- **Traductions Automatisées** : Traduisez du texte en plusieurs langues sans effort.
- **Intégration GitHub Actions** : Automatisez les traductions dans votre pipeline CI/CD.
- **Préservation du Markdown** : Conservez la syntaxe Markdown correcte pendant la traduction.
- **Traduction du Texte dans les Images** : Extrait et traduit le texte contenu dans les images.
- **Technologie LLM Avancée** : Utilisez des modèles linguistiques de pointe pour des traductions de haute qualité.
- **Intégration Facile** : S’intègre parfaitement à votre configuration de projet existante.
- **Simplifiez la Localisation** : Rationalisez la localisation de votre projet pour les marchés internationaux.

## Comment Ça Marche

![Architecture](../../imgs/architecture_241019.png)

Co-op Translator prend les fichiers Markdown et les images de votre dossier projet et les traite ainsi :

1. **Extraction du Texte** : Extrait le texte des fichiers Markdown et, si configuré (par exemple avec Azure Computer Vision), le texte intégré dans les images.
1. **Traduction par IA** : Envoie le texte extrait au LLM configuré (Azure OpenAI, OpenAI, etc.) pour traduction.
1. **Sauvegarde des Résultats** : Enregistre les fichiers Markdown traduits et les images (avec texte traduit) dans des dossiers spécifiques à chaque langue, en conservant la mise en forme originale.

## Premiers Pas

> [!NOTE]
> Bien que ce tutoriel se concentre sur les ressources Azure, vous pouvez utiliser n’importe quel modèle linguistique supporté dans la liste des [modèles et services supportés](../..).

Commencez rapidement avec la CLI ou configurez une automatisation complète avec GitHub Actions.

### Configuration Initiale

- [Configurer Azure AI](./getting_started/set-up-azure-ai.md)

### Démarrage Rapide : Ligne de Commande

Pour un démarrage rapide avec la ligne de commande :

1. Installez le package :
    ```bash
    pip install co-op-translator
    ```
2. Configurez les identifiants :
  - Créez un fichier `.env` file in your project's root directory.
  - Copy the contents from the [.env.template](../../.env.template) file into your new `.env` file.
  - Fill in the required API keys and endpoint information in your `.env` file.
3. Run Translation:
  - Navigate to your project's root directory in your terminal.
  - Execute the translate command, specifying target languages with the `-l` avec le flag :
    ```bash
    translate -l "ko ja fr"
    ```
    *(Remplacez `"ko ja fr"` with your desired space-separated language codes)*

### Detailed Usage Guides

Choose the approach that best fits your workflow:

#### 1. Using the Command Line (CLI)

- Best for: One-time translations, manual control, or integration into custom scripts.
- Requires: Local installation of Python and the `co-op-translator` package.
- Guide: [Command Line Guide](./getting_started/command-line-guide/command-line-guide.md)

#### 2. Using GitHub Actions (Automation)

- Best for: Automatically translating content whenever changes are pushed to your repository. Keeps translations consistently up-to-date.
- Requires: Setting up a workflow file (`.github/workflows`) dans votre dépôt. Aucune installation locale requise.
- Guides :
  - [Guide GitHub Actions (Dépôts Publics & Secrets Standards)](./getting_started/github-actions-guide/github-actions-guide-public.md) - À utiliser pour la plupart des dépôts publics ou personnels utilisant les secrets standards du dépôt.
  - [Guide GitHub Actions (Repos Organisation Microsoft & Configurations au Niveau Organisation)](./getting_started/github-actions-guide/github-actions-guide-org.md) - Utilisez ce guide si vous travaillez au sein de l’organisation GitHub Microsoft ou si vous devez utiliser des secrets ou runners au niveau organisation.

### Dépannage et Astuces

- [Guide de Dépannage](./getting_started/troubleshooting.md)

### Ressources Supplémentaires

- [Référence des Commandes](./getting_started/command-reference.md) : Guide détaillé de toutes les commandes et options disponibles.
- [Configuration Multi-langues](./getting_started/multi-language-support.md) : Comment ajouter un tableau avec des liens vers les versions traduites dans votre README.
- [Langues Supportées](./getting_started/supported-languages.md) : Liste des langues supportées et instructions pour en ajouter de nouvelles.
- [Mode Markdown Uniquement](./getting_started/markdown-only-mode.md) : Comment traduire uniquement le texte, sans traduction des images.

## Présentations Vidéo

Découvrez Co-op Translator à travers nos présentations _(cliquez sur l’image ci-dessous pour regarder sur YouTube)_ :

- **Open at Microsoft** : Une introduction rapide de 18 minutes et un guide express pour utiliser Co-op Translator.

  [![Open at Microsoft](../../imgs/open-ms-thumbnail.jpg)](https://www.youtube.com/watch?v=jX_swfH_KNU)

- **Microsoft Reactor** : Un guide détaillé d’une heure couvrant tout, depuis la présentation de Co-op Translator, la configuration de l’outil, son utilisation efficace, jusqu’à une démonstration en direct de ses capacités.

  [![Microsoft Reactor](../../imgs/reactor-thumbnail.jpg)](https://www.youtube.com/watch?v=boTtKVPBLAc)

## Soutenez-Nous et Favorisez l’Apprentissage Global

Rejoignez-nous pour révolutionner la façon dont le contenu éducatif est partagé dans le monde ! Donnez une ⭐ à [Co-op Translator](https://github.com/azure/co-op-translator) sur GitHub et soutenez notre mission de supprimer les barrières linguistiques dans l’apprentissage et la technologie. Votre intérêt et vos contributions ont un impact important ! Les contributions de code et suggestions de fonctionnalités sont toujours les bienvenues.

## Contribution

Ce projet accueille contributions et suggestions. Vous souhaitez contribuer à Azure Co-op Translator ? Consultez notre [CONTRIBUTING.md](./CONTRIBUTING.md) pour savoir comment aider à rendre Co-op Translator plus accessible.

## Contributeurs

[![co-op-translator contributors](https://contrib.rocks/image?repo=Azure/co-op-translator)](https://github.com/Azure/co-op-translator/graphs/contributors)

## Code de Conduite

Ce projet a adopté le [Code de Conduite Open Source Microsoft](https://opensource.microsoft.com/codeofconduct/).
Pour plus d’informations, consultez la [FAQ du Code de Conduite](https://opensource.microsoft.com/codeofconduct/faq/) ou contactez [opencode@microsoft.com](mailto:opencode@microsoft.com) pour toute question ou remarque supplémentaire.

## IA Responsable

Microsoft s’engage à aider ses clients à utiliser ses produits d’IA de manière responsable, à partager ses apprentissages et à construire des partenariats basés sur la confiance grâce à des outils comme Transparency Notes et Impact Assessments. Beaucoup de ces ressources sont disponibles sur [https://aka.ms/RAI](https://aka.ms/RAI).
L’approche de Microsoft en matière d’IA responsable repose sur nos principes d’IA : équité, fiabilité et sécurité, confidentialité et sécurité, inclusion, transparence et responsabilité.
Les modèles à grande échelle de langage naturel, d’image et de parole – comme ceux utilisés dans cet exemple – peuvent potentiellement se comporter de manière injuste, peu fiable ou offensante, ce qui peut causer des préjudices. Veuillez consulter la [note de transparence du service Azure OpenAI](https://learn.microsoft.com/legal/cognitive-services/openai/transparency-note?tabs=text) pour vous informer des risques et des limites.

La méthode recommandée pour atténuer ces risques est d’inclure un système de sécurité dans votre architecture capable de détecter et d’empêcher les comportements nuisibles. [Azure AI Content Safety](https://learn.microsoft.com/azure/ai-services/content-safety/overview) fournit une couche de protection indépendante, capable de détecter les contenus nuisibles générés par les utilisateurs et par l’IA dans les applications et services. Azure AI Content Safety inclut des API texte et image qui permettent de détecter les contenus problématiques. Nous disposons également d’un Content Safety Studio interactif qui vous permet de visualiser, explorer et tester des exemples de code pour détecter les contenus nuisibles sur différents types de données. La [documentation de démarrage rapide](https://learn.microsoft.com/azure/ai-services/content-safety/quickstart-text?tabs=visual-studio%2Clinux&pivots=programming-language-rest) suivante vous guide pour effectuer des requêtes vers le service.

Un autre aspect à prendre en compte est la performance globale de l’application. Pour les applications multi-modales et multi-modèles, la performance signifie que le système fonctionne comme vous et vos utilisateurs l’attendez, y compris en évitant de générer des résultats nuisibles. Il est important d’évaluer la performance globale de votre application en utilisant les [mesures de qualité de génération, de risque et de sécurité](https://learn.microsoft.com/azure/ai-studio/concepts/evaluation-metrics-built-in).

Vous pouvez évaluer votre application IA dans votre environnement de développement en utilisant le [prompt flow SDK](https://microsoft.github.io/promptflow/index.html). Que vous disposiez d’un jeu de données de test ou d’un objectif précis, les générations de votre application d’IA générative sont mesurées quantitativement avec des évaluateurs intégrés ou des évaluateurs personnalisés de votre choix. Pour commencer à utiliser le prompt flow sdk afin d’évaluer votre système, vous pouvez suivre le [guide de démarrage rapide](https://learn.microsoft.com/azure/ai-studio/how-to/develop/flow-evaluate-sdk). Une fois une évaluation réalisée, vous pouvez [visualiser les résultats dans Azure AI Studio](https://learn.microsoft.com/azure/ai-studio/how-to/evaluate-flow-results).

## Marques déposées

Ce projet peut contenir des marques ou logos relatifs à des projets, produits ou services. L’utilisation autorisée des marques ou logos Microsoft est soumise aux [Directives sur les marques et la marque de Microsoft](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general) et doit les respecter. L’utilisation des marques ou logos Microsoft dans des versions modifiées de ce projet ne doit pas créer de confusion ni laisser entendre un parrainage de Microsoft. Toute utilisation de marques ou logos tiers est soumise aux politiques de ces tiers.

**Avertissement** :  
Ce document a été traduit à l'aide du service de traduction automatique [Co-op Translator](https://github.com/Azure/co-op-translator). Bien que nous nous efforcions d'assurer l'exactitude, veuillez noter que les traductions automatiques peuvent contenir des erreurs ou des inexactitudes. Le document original dans sa langue d'origine doit être considéré comme la source faisant foi. Pour les informations critiques, il est recommandé de recourir à une traduction professionnelle humaine. Nous déclinons toute responsabilité en cas de malentendus ou de mauvaises interprétations résultant de l'utilisation de cette traduction.