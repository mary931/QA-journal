# Semaine 2 – Tests LibreOffice

## 🎯 Objectif
Découvrir LibreOffice Dev et commencer à exécuter quelques cas de tests manuels.

---

## 🧪 Cas de test 1 TC1 – Mettre un texte en gras dans LibreOffice Writer

**Rédigé par :** Maryline
**Date :** 24/09/2025

 Scénario 1 : Application du gras sur un mot sélectionné

**ID du Test :** GRAS-001
**Objectif :** Vérifier que la fonction "Gras" permet de mettre en valeur un texte sélectionné en le rendant visuellement plus épais.
**Priorité :** Élevée (Fonction de base essentielle)

**Préconditions :**
1. L'application LibreOffice Dev est ouverte.
2. Le module Writer est lancé avec un nouveau document vide.
3. Le texte "Baudelaire" est saisi dans le document.

**Étapes de test :**
1. Sélectionner le mot "Baudelaire" dans le document.
2. Cliquer sur le bouton "G" (Gras) dans la barre d'outils de mise en forme.

**Résultat attendu :**
Le mot "Baudelaire" s'affiche en caractères gras, contrastant visuellement avec le texte normal.

**Résultat observé :**
Le mot "Baudelaire" s'affiche correctement en caractères gras après l'application de la fonction.
**Statut :** Succès

**Notes/Observations :** Le changement est immédiat et visible. Le bouton "G" reste enfoncé (état "actif"), indiquant que la mise en forme est appliquée à la sélection.

 Scénario 2 : Désactivation de la mise en forme Gras

**ID du Test :** GRAS-002
**Objectif :** Vérifier que la fonction "Gras" peut être désactivée pour qu'un texte retrouve son apparence normale.
**Priorité :** Élevée

**Préconditions :**
1. LibreOffice Dev Writer est ouvert.
2. Le mot "Baudelaire" est saisi et affiché en gras (état issu du test GRAS-001).

**Étapes de test :**
1. Sélectionner le mot "Baudelaire" qui est déjà en gras.
2. Cliquer à nouveau sur le bouton "G" (Gras) dans la barre d'outils.

**Résultat attendu :**
Le mot "Baudelaire" retrouve une apparence normale (non gras), identique au reste du texte non formaté.

**Résultat observé :**
Le mot "Baudelaire" n'est plus en gras , le mot à retrouver son apparence normale.
**Statut :**SUCCÈS
**Notes/Observations :** Le bouton "G" n'est plus enfoncé montrant que la fonctionnalité est désactivé.

Scénario 3 : Activation du Gras via le raccourci clavier

**ID du Test :** GRAS-003
**Objectif :** Vérifier que la fonction "Gras" peut être activée via le raccourci clavier `Ctrl + B`.
**Priorité :** Moyenne (Fonction de base mais méthode d'accès secondaire)

**Préconditions :**
1. LibreOffice Dev Writer est ouvert sur un document contenant le texte "Baudelaire".
2. Le texte "Baudelaire" a une mise en forme normale (non gras).

**Étapes de test :**
1. Sélectionner le mot "Baudelaire".
2. Appuyer simultanément sur les touches `Ctrl` et `B` du clavier.

**Résultat attendu :**
Le mot "Baudelaire" s'affiche en gras (visuellement plus épais).

**Résultat observé :**
Le mot "Baudelaire" est devenu plus épais et est en gras.
**Statut :** SUCCÈS

**Notes/Observations :**
Le bouton "G" de la barre d'outils est enfoncé, confirmant la synchronisation entre le raccourci clavier et l'interface.
