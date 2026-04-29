# Local Setup

Recommended local path:

```powershell
C:\Users\toxadab\Documents\NetBeansProjects\anvikzim.ru\www\Aeo-sistem
```

---

## Clone Repository

```powershell
cd "C:\Users\toxadab\Documents\NetBeansProjects\anvikzim.ru\www"
git clone git@github.com:anvikzim-sys/Aeo-sistem.git
cd ".\Aeo-sistem"
```

---

## Copy Prepared Files

Copy the prepared files into the repository folder:

```powershell
# Example if files are unpacked into Downloads\aeo-system-github-package
Copy-Item "$HOME\Downloads\aeo-system-github-package\*" `
  "C:\Users\toxadab\Documents\NetBeansProjects\anvikzim.ru\www\Aeo-sistem" `
  -Recurse -Force
```

---

## Commit and Push

```powershell
cd "C:\Users\toxadab\Documents\NetBeansProjects\anvikzim.ru\www\Aeo-sistem"

git status
git add README.md CHANGELOG.md .gitignore docs examples
git commit -m "Add AEO-SYSTEM documentation"
git push origin main
```

---

## SSH Check

If push fails, check SSH connection:

```powershell
ssh -T git@github.com
git remote -v
```

Expected remote:

```text
git@github.com:anvikzim-sys/Aeo-sistem.git
```
