---
title: Configurer votre environnement de développement
typora-copy-images-to: ./
disableTableOfContents: true
---

Avant de commencer à créer votre premier site Gatsby, vous devez vous familiariser avec certaines technologies web de base et vous assurer que vous avez installé tous les outils logiciels requis.

## Familiarisez-vous avec la ligne de commande

La ligne de commande est une interface textuelle utilisée pour exécuter des commandes sur votre ordinateur. Vous le verrez également souvent sous le nom de terminal. Dans ce didacticiel, nous utiliserons les deux de manière interchangeable. C'est un peu comme utiliser le Finder sur un Mac ou l'Explorateur sur Windows. Finder et Explorer sont des exemples d'interfaces utilisateur graphiques (GUI). La ligne de commande est un moyen puissant et textuel d'interagir avec votre ordinateur.

<<<<<<< HEAD

Prenez le temps pour trouver et ouvrir l'interface de ligne de commande (CLI) de votre ordinateur. Selon le système d'exploitation que vous utilisez, voir [**instructions pour Mac**](http://www.macworld.co.uk/feature/mac-software/how-use-terminal-on-mac-3608274/), [**instructions pour Windows**](https://www.quora.com/How-do-I-open-terminal-in-windows) ou [**instructions pour Linux**](https://www.howtogeek.com/140679/beginner-geek-how-to-start-using-the-linux-terminal/).

## Installez Homebrew pour Node.js

Pour installer Gatsby et Node.js, il est recommandé d'utiliser [Homebrew](https://brew.sh/). Une petite configuration au début peut vous éviter quelques maux de tête plus tard !

Comment installer ou vérifier Homebrew sur votre ordinateur:

1. Ouvrez votre terminal.
1. Voir si Homebrew est installé en exécutant la commande `brew -v`. Vous devriez voir "Homebrew" et un numéro de version.
1. Sinon, téléchargez et installez-le [Homebrew avec les instructions](https://docs.brew.sh/Installation) pour votre système d'exploitation (Mac, Linux ou Windows).
1. Une fois que vous avez installé Homebrew, répétez l'étape 2 pour vérifier si il est bien installé.

### Utilisateurs Mac: installez les outils de ligne de commande Xcode

1. Ouvrez votre terminal.
1. Sur un Mac, installez les outils de ligne de commande Xcode en exécutant la commande `xcode-select --install`.
   1. Si cela échoue, téléchargez-le [directement depuis le site Apple](https://developer.apple.com/download/more/), après la connexion avec votre compte développeur de chez Apple
1. Après avoir été invité à démarrer l'installation, vous serez à nouveau invité à accepter une licence logicielle pour les outils à télécharger.

## ⌚ Installez Node.js et npm

Node.js est un environnement qui peut exécuter du code JavaScript en dehors d'un navigateur Web. Gatsby est construit avec Node.js. Pour être opérationnel avec Gatsby, vous devez avoir une version récente installée sur votre ordinateur.

_Remarque : La version Node.js minimale prise en charge par Gatsby est Node 8, mais n'hésite pas d'utiliser une version plus récente._

1. Ouvrez votre terminal.
1. Exécutez `brew update` pour vous assurer que vous disposez de la dernière version de Homebrew.
1. Exécutez cette commande pour installer Node et npm en une seule fois: `brew install node`

Une fois que vous avez suivi les étapes d'installation, assurez-vous que tout a été correctement installé:

### Vérifiez votre installation Node.js

1.  Ouvrez votre terminal.
2.  Exécutez `node --version`. (Si vous êtes nouveau avec les lignes de commande, Exécutez `command`” veux dire “type `node --version` dans l'invite de commande, et appuyez sur la touche Entrée”. À partir de là, c'est ce que nous entendons par Exécutez `command`”).
3.  Exécutez `npm --version`.
=======
Take a moment to locate and open up the command line interface (CLI) for your computer. Depending on which operating system you are using, see [**instructions for Mac**](http://www.macworld.co.uk/feature/mac-software/how-use-terminal-on-mac-3608274/), [**instructions for Windows**](https://www.lifewire.com/how-to-open-command-prompt-2618089) or [**instructions for Linux**](https://www.howtogeek.com/140679/beginner-geek-how-to-start-using-the-linux-terminal/).

_Note: If you’re new to the command line, "running" a command, means writing a given set of instructions in your command prompt, and hitting the Enter key”. Commands will be shown in a highlighted box, something like `node --version`, but not every highlighted box is a command! If something is a command it will be mentioned as something you have to run/execute._

## Install Node.js for your appropriate operating system

Node.js is an environment that can run JavaScript code outside of a web browser. Gatsby is built with Node.js. To get up and running with Gatsby, you’ll need to have a recent version installed on your computer. npm comes bundled with Node.js so if you don't have npm, chances are that you don't have Node.js either.

### Mac instructions

To install Gatsby and Node.js on a Mac, it is recommended to use [Homebrew](https://brew.sh/). A little set-up in the beginning can save you from some headaches later on!

#### How to install or verify Homebrew on your computer:

1. Open your Terminal.
1. See if Homebrew is installed by running `brew -v`. You should see "Homebrew" and a version number.
1. If not, download and install [Homebrew with the instructions](https://docs.brew.sh/Installation).
1. Once you've installed Homebrew, repeat step 2 to verify.

#### Install Xcode Command Line Tools:

1. Open your Terminal.
1. Install Xcode Command line tools by running `xcode-select --install`.
   - If that fails, download it [directly from Apple's site](https://developer.apple.com/download/more/), after signing-in with an Apple developer account
1. After being prompted to start the installation, you'll be prompted again to accept a software license for the tools to download.

#### Install Node

1. Open your Terminal
2. Run `brew install node`
   - If you don't want to install it through Homebrew, download the latest Node.js version from [the official Node.js website](https://nodejs.org/en/), double click on the downloaded file and go through the installation process.

### Windows Instructions

- Download and install the latest Node.js version from [the official Node.js website](https://nodejs.org/en/)

### Linux Instructions

Install nvm (Node Version Manager) and needed dependencies. nvm is used to manage Node.js and all its associated versions.

_💡 If when installing a package, it asks for confirmation, type `y` and press enter._

#### Ubuntu, Debian, and other `apt` based distros:

1. Run `sudo apt update` and then `sudo apt -y upgrade` to make sure your Linux distribution is ready to go.
2. Run `sudo apt-get install curl` to install curl which allows you to transfer data and download additional dependencies.
3. After it finishes installing, run `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash` to download the latest nvm version.
4. To confirm this has worked, use the following command. `nvm --version`. The output should be a version number.
5. [Set default Node.js version](#set-default-nodejs-version)

#### Arch, Manjaro and other `pacman` based distros:

1. Run `sudo pacman -Sy` to make sure your distribution is ready to go.
2. These distros come installed with curl, so you can use that to download nvm.
   `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash`
3. Before using nvm, you need to install additional dependencies by running `sudo pacman -S grep awk tar`.
4. To confirm this has worked, use the following command. `nvm --version`. The output should be a version number.
5. [Set default Node.js version](#set-default-nodejs-version)

#### Fedora, RedHat, and other `dnf` based distros:

1. These distros come installed with curl, so you can use that to download nvm.
   `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash`
2. To confirm this has worked, use the following command. `nvm --version`. The output should be a version number.
3. [Set default Node.js version](#set-default-nodejs-version)

If the Linux distribution you are using is not listed here, please find instructions on the web.

#### Set default Node.js version

When nvm is installed, it does not default to a particular node version. You’ll need to install the version you want and give nvm instructions to use it. This example uses the latest release of version 10, but more recent version numbers can be used instead.

```shell
nvm install 10
nvm use 10
```

To confirm that this worked, you can run `npm --version` and `node --version`. The output should look similar to the screenshot below, showing version numbers in response to the commands.
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7

La sortie de chacune de ces commandes doit être un numéro de version. Vos versions peuvent ne pas être les mêmes que celles illustrées ci-dessous! Si la saisie de ces commandes ne vous montre pas de numéro de version, revenez en arrière et assurez-vous d'avoir installé Node.js.

<<<<<<< HEAD
![Vérifier les versions de node et npm dans le terminal](01-node-npm-versions.png)
=======
Once you have followed the installation steps and you have checked everything is installed properly, you can continue to the next step.

## Install Git
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7

## Installer Git

Git est un système de contrôle de version distribué gratuit et open source conçu pour gérer tout, des petits aux très grands projets avec rapidité et efficacité. Lorsque vous installez un site "starter" Gatsby, Gatsby utilise Git en arrière-plan pour télécharger et installer les fichiers requis pour votre starter. Vous devrez avoir installé Git pour configurer votre premier site Gatsby.

Les étapes pour télécharger et installer Git dépendent de votre système d'exploitation. Suivez le guide de votre système:

- [Installer Git sur macOS](https://www.atlassian.com/git/tutorials/install-git#mac-os-x)
- [Installer Git sur Windows](https://www.atlassian.com/git/tutorials/install-git#windows)
- [Installer Git sur Linux](https://www.atlassian.com/git/tutorials/install-git#linux)

## Utilisation de la CLI Gatsby

L'outil CLI de Gatsby vous permet de créer rapidement de nouveaux sites propulsés par Gatsby et d'exécuter des commandes pour développer des sites Gatsby. Il s'agit d'un package npm publié.

La CLI Gatsby est disponible via npm et doit être installée globalement en exécutant `npm install -g gatsby-cli`.

_**Remarque**: lorsque vous installez Gatsby et l'exécutez pour la première fois, vous verrez un court message vous informant des données d'utilisation anonymes qui sont collectées pour les commandes Gatsby, vous pouvez en savoir plus sur la façon dont ces données sont extraites et utilisées dans le [doc de télémétrie](/docs/telemetry)._

Pour voir les commandes disponibles, exécutez `gatsby --help`.

![Vérifier les commandes Gatsby dans le terminal](05-gatsby-help.png)

> 💡 Si vous ne parvenez pas à exécuter correctement l'interface de ligne de commande Gatsby en raison d'un problème d'autorisations, vous souhaiterez peut-être consulter la [documentation npm sur la fixation des autorisations](https://docs.npmjs.com/getting-started/fixing-npm-permissions), ou [ce guide](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo.md).

## Créer un site Gatsby

Vous êtes maintenant prêt à utiliser l'outil CLI Gatsby pour créer votre premier site Gatsby. À l'aide de l'outil, vous pouvez télécharger des "starters" (sites partiellement construits avec une configuration par défaut) pour vous aider à accélérer la création d'un certain type de site. Le démarreur "Hello World" que vous utiliserez ici est un démarreur avec l'essentiel nécessaire pour un site Gatsby.

1.  Ouvrez votre terminal.
2.  Exécutez `gatsby new hello-world https://github.com/gatsbyjs/gatsby-starter-hello-world`. (_Remarque: En fonction de votre vitesse de téléchargement, le temps que cela prendra variera. Par souci de concision, le gif ci-dessous a été suspendu pendant une partie de l'installation_).
3.  Exécutez `cd hello-world`.
4.  Exécutez `gatsby develop`.

<video controls="controls" autoplay="true" loop="true">
  <source type="video/mp4" src="./03-create-site.mp4" />
<<<<<<< HEAD
  <p>Désolé! Votre navigateur ne prend pas en charge cette vidéo.</p>
=======
  <p>Sorry! Your browser doesn't support this video.</p>
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7
</video>

Qu'est-ce qui vient de se passer?

```shell
gatsby new hello-world https://github.com/gatsbyjs/gatsby-starter-hello-world
```

- `new` est une commande gatsby pour créer un nouveau projet Gatsby.
- Ici, `hello-world` est un titre arbitraire - vous pouvez choisir n'importe quoi. L'outil CLI placera le code de votre nouveau site dans un nouveau dossier appelé “hello-world”.
- Enfin, l'URL GitHub spécifiée pointe vers un référentiel de code qui contient le code de démarrage que vous souhaitez utiliser.

```shell
cd hello-world
```

- Cela dit : 'Je veux changer les répertoires («cd») en sous-dossier «hello-world». Chaque fois que vous souhaitez exécuter des commandes pour votre site, vous devez être dans le contexte de ce site (alias votre terminal doit être pointé vers le répertoire où réside le code de votre site).

```shell
gatsby develop
```

- Cette commande démarre un serveur de développement. Vous pourrez voir et interagir avec votre nouveau site dans un environnement de développement local (sur votre ordinateur, non publié sur Internet).

<<<<<<< HEAD
### Affichez votre site localement
=======
Open up a new tab in your browser and navigate to `http://localhost:8000/`
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7

Ouvrez un nouvel onglet dans votre navigateur et accédez à [**http://localhost:8000**](http://localhost:8000/).

![Vérifier la page d'accueil](04-home-page.png)

<<<<<<< HEAD
Félicitations! C'est le début de votre tout premier site Gatsby!🎉

Vous pourrez visiter le site localement à [**_http://localhost:8000_**](http://localhost:8000/) tant que votre serveur de développement est en cours d'exécution. C’est le processus que vous avez commencé en exécutant la commande `gatsby develop`. Pour arrêter l'exécution de ce processus (ou pour «arrêter l'exécution du serveur de développement»), revenez à la fenêtre de votre terminal, maintenez enfoncée la touche "control" puis appuyez sur «c» (ctrl-c). Pour le redémarrer, lancez à nouveau la commande `gatsby develop`!
=======
You’ll be able to visit the site locally at `http://localhost:8000/` for as long as your development server is running. That’s the process you started by running the `gatsby develop` command. To stop running that process (or to “stop running the development server”), go back to your terminal window, hold down the “control” key, and then hit “c” (ctrl-c). To start it again, run `gatsby develop` again!

**Note:** If you are using VM setup like `vagrant` and/or would like to listen on your local IP address, run `gatsby develop --host=0.0.0.0`. Now, the development server listens on both `http://localhost` and your local IP.
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7

**Remarque:** Si vous utilisez une configuration VM comme`vagrant` et / ou souhaitez écouter sur votre adresse IP locale, exécutez `gatsby develop -- --host=0.0.0.0`. Maintenant, le serveur de développement écoute à la fois sur «localhost» et sur votre IP locale.

## Configurer un éditeur de code

Un éditeur de code est un programme spécialement conçu pour éditer du code informatique. Il y en a beaucoup là-bas.

### Télécharger VS Code

La documentation de Gatsby inclut parfois des captures d'écran qui ont été prises dans VS Code, donc si vous n'avez pas encore d'éditeur de code préféré, l'utilisation de VS Code s'assurera que votre écran ressemble exactement aux captures d'écran du didacticiel et des documents. Si vous choisissez d'utiliser VS Code, visitez le site [VS Code](https://code.visualstudio.com/#alt-downloads) et téléchargez la version appropriée pour votre plate-forme.

### Installez le plugin Prettier

Nous vous recommandons également d'utiliser [Prettier](https://github.com/prettier/prettier), un outil qui permet de formater votre code pour éviter les erreurs.

<<<<<<< HEAD
Vous pouvez utiliser Prettier directement dans votre éditeur à l'aide du [plugin Prettier VS Code](https://github.com/prettier/prettier-vscode):
1.  Ouvrez la vue des extensions sur VSCode (View => Extensions).
2.  Recherchez "Prettier - Code formatter".
3.  Cliquez sur "Install". (Après l'installation, vous serez invité à redémarrer VS Code pour activer l'extension. Les versions plus récentes de VS Code activeront automatiquement l'extension après le téléchargement.)
=======
1.  Open the extensions view on VS Code (View => Extensions).
2.  Search for "Prettier - Code formatter".
3.  Click "Install". (After installation, you'll be prompted to restart VS Code to enable the extension. Newer versions of VS Code will automatically enable the extension after download.)
>>>>>>> fd3df38d5351bfbf1bf86cb9e0c8cc80dc9ba2a7

> 💡 Si vous n'utilisez pas VS Code, consultez la documentation Prettier pour [les intructions d'installation](https://prettier.io/docs/en/install.html) ou [autres intégrations d'éditeur](https://prettier.io/docs/en/editors.html).

## ➡️ Et après?

Pour résumer, dans cette section vous:

- Connaître la ligne de commande et comment l'utiliser
- Installation et apprentissage de Node.js et de l'outil CLI npm, du système de contrôle de version Git et de l'outil CLI Gatsby
- Généré un nouveau site Gatsby à l'aide de l'outil CLI Gatsby
- Exécutez le serveur de développement Gatsby et visitez votre site localement
- Téléchargez un éditeur de code
- Installation d'un formateur de code appelé Prettier

Maintenant, passez à [**apprendre à connaître les blocs de construction de Gatsby**](/tutorial/part-one/).

## Références

### Aperçu des technologies de base

Il n’est pas nécessaire d’être déjà expert en la matière - sinon, ne vous inquiétez pas! Vous en apprendrez beaucoup au cours de cette série de didacticiels. Voici quelques-unes des principales technologies Web que vous utiliserez lors de la création d'un site Gatsby:

- **HTML**: Un langage de balisage que chaque navigateur Web est capable de comprendre. Il signifie HyperText Markup Language. HTML donne à votre contenu Web une structure d'information universelle, définissant des éléments tels que des titres, des paragraphes, etc.
- **CSS**: Un langage de présentation utilisé pour styliser l'apparence de votre contenu Web (polices, couleurs, mise en page, etc.). Il signifie feuilles de style en cascade.
- **JavaScript**: Un langage de programmation qui nous aide à rendre le Web dynamique et interactif.
- **React**: Une librairie (construite avec JavaScript) pour créer des interfaces utilisateur. C'est le cadre que Gatsby utilise pour créer des pages et structurer le contenu.
- **GraphQL**: Un langage de requête qui vous permet d'extraire des données dans votre site Web. Il s'agit de l'interface que Gatsby utilise pour gérer les données du site.

### Qu'est-ce qu'un site Web?

Pour une introduction complète à ce qu'est un site Web - y compris une introduction à HTML et CSS - consultez “[**Création de votre première page Web**](https://learn.shayhowe.com/html-css/building-your-first-web-page/)”. C'est un excellent endroit pour commencer à découvrir le Web. Pour une introduction plus pratique à [**HTML**](https://www.codecademy.com/learn/learn-html), [**CSS**](https://www.codecademy.com/learn/learn-css), et [**JavaScript**](https://www.codecademy.com/learn/introduction-to-javascript), consultez les tutoriels de Codecademy. [**React**](https://reactjs.org/tutorial/tutorial.html) et [**GraphQL**](http://graphql.org/graphql-js/) ont également leurs propres tutoriels d'introduction.

### En savoir plus sur la ligne de commande

Pour une excellente introduction à l'utilisation de la ligne de commande, consultez [**Tutoriel Command Line de Codecademy**](https://www.codecademy.com/courses/learn-the-command-line/lessons/navigation/exercises/your-first-command) pour les utilisateurs Mac et Linux, et [**ce tutorial**](https://www.computerhope.com/issues/chusedos.htm) pour les utilisateurs de Windows. Même si vous êtes un utilisateur Windows, la première page du didacticiel Codecademy est une lecture précieuse. Il explique ce qu'est la ligne de commande, pas seulement comment s'interfacer avec elle.

### En savoir plus sur npm

npm est un gestionnaire de packages JavaScript. Un package est un module de code que vous pouvez choisir d'inclure dans vos projets. Si vous venez de télécharger et d'installer Node.js, npm a été installé avec!

npm a trois composants distincts: le site Web npm, le registre npm et l'interface de ligne de commande (CLI) npm.

- Sur le site Web de npm, vous pouvez parcourir les packages JavaScript disponibles dans le registre npm.
- Le registre npm est une grande base de données d'informations sur les packages JavaScript disponibles sur npm.
- Une fois que vous avez identifié le package souhaité, vous pouvez utiliser la CLI npm pour l'installer dans votre projet ou globalement (comme les autres outils CLI). La CLI npm est ce qui parle au registre.
- vous n'interagissez généralement qu'avec le site Web npm ou la CLI npm.

> 💡 Découvrez l'introduction de npm, “[**Qu'est-ce que npm?**](https://docs.npmjs.com/getting-started/what-is-npm)”.

### En savoir plus sur Git

Vous n'aurez pas besoin de connaître Git pour terminer ce tutoriel, mais c'est un outil très utile. Si vous souhaitez en savoir plus sur le contrôle de version, Git et GitHub, consultez GitHub [Manuel Git](https://guides.github.com/introduction/git-handbook/).
