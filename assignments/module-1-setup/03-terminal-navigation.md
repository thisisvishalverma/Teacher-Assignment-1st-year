# Assignment 3: Terminal Navigation Practice

These examples use Windows PowerShell. Run them from the project folder in a terminal. The final step, opening VS Code, is left for you to do on your computer.

| Goal | PowerShell command |
|---|---|
| Show the current folder | `Get-Location` |
| List visible items | `Get-ChildItem` |
| Include hidden items | `Get-ChildItem -Force` |
| Make a folder | `New-Item -ItemType Directory practice` |
| Enter a folder | `Set-Location practice` |
| Create an empty file | `New-Item index.html -ItemType File` |
| Make nested folders | `New-Item -ItemType Directory css, images` |
| Go up one folder | `Set-Location ..` |
| Copy a file | `Copy-Item index.html backup.html` |
| Rename a file | `Rename-Item backup.html old.html` |
| Print a file | `Get-Content index.html` |
| List a folder tree | `Get-ChildItem -Recurse` |
| Open this folder in VS Code | `code .` |

## Practice sequence

From this assignment's folder, create `practice-site`, then add `css`, `images`, `index.html`, and `css/style.css`. Enter `css`, return to the site folder with one `..` command, list the tree, and rename `index.html` to `home.html` and back. Remove only the practice files you created after checking the paths. Finally, run `code .` yourself to open the folder in VS Code.

## Record your run

Write the commands you actually entered below. Keep your own terminal screenshot if your teacher requests proof.

```text
_Record your commands here after running the practice._
```
