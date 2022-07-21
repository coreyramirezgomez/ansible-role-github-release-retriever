Github Release Retriever
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

Returns github_release_retriever_downloads register with results of get_url.
Access downloads by reviewing the structure here: https://docs.ansible.com/ansible/latest/collections/ansible/builtin/get_url_module.html#return-values


Example Playbook
----------------
    ---
    - hosts: all
      roles:
        - role: coreyramirezgomez.github_release_retriever
          github_release_retriever_project: "munki/munki"
          github_release_retriever_download_path: "/tmp/"