# 📸 Guide : Ajouter votre photo au site

## Méthode simple (Recommandée)

### Option 1 : Copier manuellement la photo
1. **Localisez votre photo** (celle avec la veste bleue que vous avez partagée)
2. **Copiez-la** dans le dossier `images/` de ce projet
3. **Renommez-la** en `fondateur.jpg`
4. **Ouvrez** `index.html` dans votre navigateur
5. ✅ Votre photo apparaîtra automatiquement dans la section "À propos" !

### Option 2 : Utiliser PowerShell (Automatique)
Si votre photo est sur le bureau ou dans un autre dossier, utilisez cette commande :

```powershell
# Remplacez le chemin par l'emplacement réel de votre photo
Copy-Item "C:\Users\DANISKISS\Downloads\votre-photo.jpg" -Destination ".\images\fondateur.jpg"
```

## Vérification
Une fois la photo ajoutée :
1. Ouvrez `index.html` dans votre navigateur
2. Faites défiler jusqu'à la section "À propos"
3. Vous devriez voir votre photo professionnelle dans la galerie du fondateur

## En cas de problème
- **La photo ne s'affiche pas ?**
  - Vérifiez que le fichier s'appelle exactement `fondateur.jpg` (pas `fondateur.JPG` ou `fondateur.jpeg`)
  - Vérifiez qu'il est bien dans le dossier `images/`
  - Actualisez la page (F5 ou Ctrl+R)

- **Vous voulez utiliser un autre nom de fichier ?**
  - Modifiez la ligne dans `index.html` : `<img src="./images/fondateur.jpg">`
  - Remplacez `fondateur.jpg` par le nom de votre fichier

## Pousser sur GitHub après ajout
Une fois votre photo ajoutée :

```powershell
git add images/fondateur.jpg
git commit -m "Ajout photo du fondateur"
git push origin main
```

Votre site sur GitHub sera mis à jour avec votre vraie photo ! 🚀
