Role Name
=========

Ansible task sequence to retrieve release artifacts from github projects.

Requirements
------------

None.

Role Variables
--------------

See defaults/main.yml for all variables.
Required:
  - github_release_retriever_project
  - github_release_retriever_download_path



Example Playbook
----------------

  ---
  - hosts: all
    roles:
      - role: coreyramirezgomez.github_release_retriever
        github_release_retriever_project: "munki/munki"
        github_release_retriever_download_path: "/tmp/"