Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
------------------------------------
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
