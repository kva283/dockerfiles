# Image : ansible-core

## Détail de l'image
- Contenu de l'image :
  - OS : Debian 13 (Trixie)
  - Python : 3.13.6
  - Ansible-core : 2.18.8

- L'image offre une version d'`ansible-core` installée via pip.
- `ansible-core` est la version la plus minimaliste qui soit pour exécuter Ansible.
- Dockerfile validé via `HadoLint`.

## Build de l'image
docker build . -t ansible-core:2.18.8
