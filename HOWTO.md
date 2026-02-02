# Guide d’installation et d’exécution

Ce document explique comment installer et lancer le projet **Jeu 2D JavaFX (type Terraria)**,  
soit via un **IDE**, soit directement en **ligne de commande avec Maven**.

---

## Prérequis

Avant de commencer, assurez-vous d’avoir installé :

- **Java JDK 17** (ou version compatible)
- **Maven**
- **Git**

### Vérification des installations

Dans un terminal (cmd, PowerShell, bash) :

```bash
java -version
mvn -version
git --version
```

Si une commande n’est pas reconnue, l’outil correspondant n’est pas installé ou mal configuré dans le `PATH`.

### Récupération du projet

Cloner le dépôt Github :

```bash
git clone https://github.com/wael11111/Java_Terraria.git
cd Java_Terraria
```

## Lancement du projet avec Maven (recommandé)

Le projet utilise Maven et JavaFX.  
Depuis la racine du projet :

`mvn clean javafx:run`

Cette commande nettoie les fichiers de compilation précédents, 
compile le projet, télécharge les dépendances nécessaires et
lance automatiquement l’application JavaFX.

Aucune configuration supplémentaire n’est requise.

## Lancement du projet via un IDE (optionnel)

Le projet peut également être lancé depuis un IDE Java.

### Avec IntelliJ IDEA (recommandé)

- **Ouvrir IntelliJ IDEA**
- **Open → sélectionner le dossier du projet**
- **Attendre** l’import Maven et le téléchargement des dépendances
- **Lancer** la classe principale : `Lancement`

#### Autres IDE

- **Eclipse**
- **VS Code** (avec extensions Java)

Le projet étant basé sur Maven, l’import est généralement automatique.

## Problèmes courants

### "mvn n’est pas reconnu"
Maven n’est pas installé ou pas ajouté au `PATH`.

Vérifier l’installation avec `mvn -version`.

### Erreur liée à JavaFX

Vérifier que les dépendances JavaFX sont bien présentes dans le `pom.xml`.

Vérifier la version de Java utilisée (`java -version`).

### Mauvaise version de Java

Le projet nécessite **Java 17** (ou version définie dans le projet).

Vérifier la version active sur votre machine.

## Informations complémentaires

* Des documents supplémentaires sont disponibles dans le dossier `docs/`
* Un journal de bord est également fourni pour illustrer l’évolution du projet