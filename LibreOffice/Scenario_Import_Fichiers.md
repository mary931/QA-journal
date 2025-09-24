 Scénario de Test : Import de fichiers dans LibreOffice Dev Writer

**Objectif du Scénario :** Vérifier la robustesse et la compatibilité de la fonctionnalité d'import de fichiers, notamment avec les formats anciens et les cas limites.

## 🧪 Cas de Test 1 : TC-IMPORT-001 - Ouverture d'un fichier .doc (ancien format)

**ID :** TC-IMPORT-001
**Objectif :** Vérifier la rétrocompatibilité de l'application en testant l'ouverture d'un fichier au format .doc ancien.
**Priorité :** Élevée (Garantir l'accès aux documents historiques)

**Préconditions :**
1. Le fichier `vieux_souvenir.doc` a été créé et enregistré au format Word 97-2003.
2. L'application LibreOffice Dev Writer est ouverte sur un nouveau document vide.

**Étapes de test :**
1. Dans le menu, cliquer sur `Fichier` > `Ouvrir...`.
2. Naviguer jusqu'au fichier `vieux_souvenir.doc` et le sélectionner.
3. Cliquer sur le bouton `Ouvrir`.

**Résultat attendu :**
Le fichier `vieux_souvenir.doc` s'ouvre correctement dans la fenêtre active. Le texte "Ceci est un test d'import d'un ancien format." est lisible et intact.

**Résultat observé :**
Le fichier s'ouvre correctement et instantanément dans la fenêtre principale de l'application. Le contenu est affiché clairement et fidèlement.
**Statut :** SUCCÈS (Fonctionnalité principale validée)

**Notes/Observations :**
- **Anomalie mineure (UI) :** Les boutons "Aligner à gauche" et "De gauche à droite" de la barre d'outils sont enfoncés par défaut à l'ouverture du fichier `.doc`. Ce comportement est inattendu et pourrait indiquer un formatage par défaut spécifique à l'import des anciens formats.
