# Image : ansible-core

## Détail de l'image
- Contenu de l'image :
  - OS : Debian 13 (Trixie)
  - Python : 3.13.6
  - Ansible : 11.9.0

- L'image offre une version d'Ansible complète installée via pip. Cette version contient tous les modules de base d'Ansible.
- Dockerfile validé via `HadoLint`.

## Build de l'image
docker build . -t ansible-full:11.9.0
