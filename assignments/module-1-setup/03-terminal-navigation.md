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
Get-Location
Get-ChildItem
Get-ChildItem -Force
New-Item -ItemType Directory practice-site
Set-Location practice-site
New-Item -ItemType Directory css, images
New-Item -ItemType File index.html
New-Item -ItemType File css/style.css
Set-Location css
Set-Location ..
Get-ChildItem -Recurse
Rename-Item index.html home.html
Rename-Item home.html index.html
Set-Location ..
Get-Location
Get-ChildItem .\practice-site -Recurse
Resolve-Path .\practice-site
if ((Resolve-Path .\practice-site).Path -eq 'C:\Users\dell\Documents\html-css-45-practicals\assignments\module-1-setup\practice-site') { Remove-Item -LiteralPath 'C:\Users\dell\Documents\html-css-45-practicals\assignments\module-1-setup\practice-site' -Recurse -Force }
Test-Path .\practice-site
code .
code .
code .
```

The practice folder was removed after its resolved path was checked. `Test-Path` returned `False`. `code .` was run from this assignment folder; VS Code was detected as running afterward, but its window could not be visually verified because computer-use capture timed out. Keep a terminal screenshot only if your teacher requests one.
