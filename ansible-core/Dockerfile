# Utiliser une image de base Python légère
FROM python:3-slim

# Mettre à jour le gestionnaire de paquets et installer les dépendances nécessaires
RUN apt update && \
    apt install -y --no-install-recommends \
    sshpass \
    openssh-client

# Installer Ansible via pip
RUN pip install --no-cache-dir ansible-core

# Declaration chemin vers conf Ansible
ENV ANSIBLE_CONFIG="./ansible.cfg"

# Créer un répertoire de travail
WORKDIR /ansible

# Copier les fichiers Ansible dans le répertoire de travail (si besoin)
# COPY ./ansible /ansible

# Définir le point d'entrée par défaut (si besoin)
# ENTRYPOINT ["ansible-playbook"]

# Définir la commande par défaut
CMD ["ansible", "--version"]
