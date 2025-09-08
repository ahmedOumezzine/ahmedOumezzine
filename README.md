# 🧠 Mini Analyseur de Code C# — Projet Éducatif

> Un outil web interactif pour analyser la qualité du code C# en temps réel — parfait pour l’apprentissage, la revue de code ou l’amélioration des pratiques pour les développeurs.

![Mini Analyseur C#](https://via.placeholder.com/800x400?text=Mini+Analyseur+C%23+Interface)

---

## 🎯 Fonctionnalités

Cet outil analyse ton code C# et te donne des **retours immédiats** sur :

✅ **Nommage** — Respect des conventions (PascalCase, _camelCase)  
✅ **Complexité cyclomatique** — Score sur 20 + niveaux (Faible → Critique)  
✅ **Variables inutilisées** — Détection des variables déclarées mais non utilisées  
✅ **Visibilité** — Éviter les champs publics, suggérer `private` implicite  
✅ **Console.WriteLine** — Détecter les `Console.WriteLine` (à éviter en prod)  
✅ **Documentation XML** — Vérifier la présence de `/// <summary>`

---

## 🚀 Démonstration

Colle ton code C# → Clique sur “Analyser” → Obtenez des retours en temps réel :

- 🔴 **Erreurs** (ex: mauvais nommage)
- 🟠 **Avertissements** (ex: complexité élevée, variables inutilisées)
- 🔵 **Suggestions** (ex: documentation manquante, visibilité à ajuster)

Si aucune erreur n’est détectée, le système indiquera que le code est de bonne qualité et prêt à être utilisé ou revu.

---

## 🧰 Technologies utilisées

- **Frontend** : HTML, CSS, Bootstrap 5, JavaScript, Monaco Editor
- **Backend** : ASP.NET Core (C#)
- **Analyseurs** : Regex, parsing manuel, règles métier
- **UI/UX** : Design responsive, modals Bootstrap, surlignage dynamique

---

## 📦 Installation & Exécution

### Prérequis

- [.NET 6.0 ou +](https://dotnet.microsoft.com/download)  
- [Node.js (optionnel, pour extensions)](https://nodejs.org/)

### Étapes

1. Clone le dépôt :
   ```bash
   git clone https://github.com/ahmedOumezzine/CSharpCodeAnalyzer.git
   cd CSharpCodeAnalyzer
   ```
2. Restaure les packages :
   ```bash
   dotnet restore
   ```
3. Lancer l’application :
   ```bash
   dotnet run
   ```
4. Ouvrir le navigateur :
   ```
   https://localhost:5001
   ```

---

## 🧪 Projets phares

- 🔧 **[EFCore.Repository](https://github.com/ahmedOumezzine/EFCore.Repository)** — Méthodes génériques pour simplifier les opérations CRUD avec Entity Framework Core.
- 🎓 **Plateforme d’apprentissage** *(privée)* — Aide les candidats à préparer leurs examens avec des résumés, quiz interactifs et simulateurs.
- 📰 **[Blog IT personnalisé](https://blog.oumezzine.com)** — Plateforme blog moderne développée avec ASP.NET Core, système de gestion de contenu intégré.

### 💻 Autres projets GitHub
- **[Editing-a-Resource-File - Web Application](https://github.com/ahmedOumezzine/Editing-a-Resource-File---web-application)** — Lire et modifier facilement des fichiers `.resx` pour la gestion multilingue.
- **[GravatarHelper.AspNetMVC](https://github.com/ahmedOumezzine/GravatarHelper.AspNetMVC)** — Bibliothèque pour intégrer les images Gravatar dans les applications ASP.NET MVC.
- **[Puppeteer-Sharp](https://github.com/ahmedOumezzine/Puppeteer-Sharp)** — Automatisation du navigateur et génération de PDF pour les applications .NET.
- **[Gallery-Photos](https://github.com/ahmedOumezzine/Gallery-Photos)** — Galerie photo responsive avec ASP.NET Core.
- **[FlashMessage.Library](https://github.com/ahmedOumezzine/FlashMessage.Library)** — Affichage de messages flash dans les applications ASP.NET Core.
- **[Microfrontends Tutorial](https://github.com/ahmedOumezzine/microfrontends-tutorial)** — Guide pratique pour implémenter l’architecture des micro-frontends.
- **[CSharpCodeAnalyzer](https://github.com/ahmedOumezzine/CSharpCodeAnalyzer)** — Analyseur de code C# en ligne avec retours sur la qualité du code et recommandations.

---

## 📚 Exemples de tests

Colle ces codes pour tester :

**Test Nommage**
```csharp
public class Test
{
    public void badName() { } // → Erreur : PascalCase
    private string field;     // → Warning : _camelCase
}
```

**Test Complexité**
```csharp
public void ComplexMethod()
{
    for (int i = 0; i < 10; i++)
    {
        if (i % 2 == 0 && i > 5 || i < 3)
        {
            switch (i)
            {
                case 1: break;
                case 2: break;
            }
        }
    }
} // → Complexité : 10/20 (Moyenne) ⚠️
```

**Test Documentation XML**
```csharp
public class Sample
{
    /// <summary>
    /// Effectue un calcul
    /// </summary>
    public int Compute() { return 0; }
}
```

---

## 🐛 Signaler un bug / issue

Si vous trouvez un bug ou souhaitez suggérer une amélioration, merci de créer un ticket ici :  
🔗 [Issues GitHub](https://github.com/ahmedOumezzine/CSharpCodeAnalyzer/issues)

---

## 📬 Contact

- ✉️ **Email** : ahmedoumezzine@outlook.fr  
- 🔗 **LinkedIn** : [https://www.linkedin.com/in/ahmedoumezzine/](https://www.linkedin.com/in/ahmedoumezzine/)

---

Merci d’avoir visité ce projet !  
👉 Explorez le code, testez vos scripts C# et améliorez vos pratiques de développement.

