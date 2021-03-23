# add-to-ad
---
## Déploiement de l'ajout des serveurs Linux dans le **domaine AD** via **Ansible**

Le déploiement se base sur le travail proposé par [***server-word***](https://www.server-world.info/en/note?os=Ubuntu_20.04&p=realmd)

---
## Rôle Ansible
Ci-dessous vous avez l'organisation des rôles et des playbooks Ansibles
.
├── README.md
├── add_to_ad
│   ├── README.md
│   ├── defaults
│   │   └── main.yml
│   ├── tasks
│   │   ├── main.yml
│   │   └── sssd.yml
│   └── vars
│       └── main.yml
└── golden_ad.yml

1. Le script *golden_ad.yml* gère le déploiement de l'ensemble des rôles
2. Le répertoire *tasks* contient les tâches qui vont être jouées par Ansible.
3. les mots de passe sont chiffrés via ***ansible-vault*** dans le fichier *main.yml* du répertoire *defaults*
4. Le repertoire *vars* contient les variables utilisées. 

Le second fichier README.md donne des informations sur le déploiement.
