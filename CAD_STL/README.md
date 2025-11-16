# CAD and STL Files

Dieser Ordner enthält die 3D-Modelldateien (STL) und CAD-Quellen für das Myoelectric Hand Prosthesis Project.

Anleitung:
- Lege deine `.stl`-Dateien direkt in dieses Verzeichnis oder in Unterordner (z. B. `STL/` oder `SourceCAD/`).
- Für große Binärdateien (größer als ~50 MB) verwende bitte Git LFS (siehe unten).

Empfehlungen:
- Verwende aussagekräftige Dateinamen (z. B. `finger_index.stl`, `palm_v2.stl`).
- Füge Quell-CAD-Dateien (z. B. Fusion360, SolidWorks) in `SourceCAD/` ein, wenn möglich.

Git LFS Hinweis:
- GitHub hat eine harte Grenze von 100 MB pro Datei. Für große STL-Dateien installiere Git LFS:

  ```bash
  git lfs install
  git lfs track "*.stl"
  git add .gitattributes
  git add CAD_STL/*.stl
  git commit -m "Add large STL files via Git LFS"
  git push origin main
  ```

Wenn du möchtest, kann ich Git LFS hier initialisieren und Beispielbefehle ausführen.

Wenn du die STL-Dateien jetzt hast, kannst du sie per Drag & Drop in VS Code in dieses Verzeichnis legen, oder die Dateien lokal mit `cp`/`scp` in `/workspaces/Myoelectric_Hand_Prosthesis_Project/CAD_STL/` kopieren.
