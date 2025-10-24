# Utiliser une image de base Python légère
FROM python:3.13-slim-trixie

# Mettre à jour le gestionnaire de paquets et installer les dépendances nécessaires
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        sshpass \
        openssh-client \
        git && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Installer Ansible via pip
RUN pip install --no-cache-dir ansible==11.9.0

# Declaration chemin vers conf Ansible
ENV ANSIBLE_CONFIG="./ansible.cfg"

# Créer un répertoire de travail
WORKDIR /ansible

# Définir la commande par défaut
CMD ["ansible", "--version"]
