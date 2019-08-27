ansible-git-clone
=========

Use this role to clone git repositories.


Role Variables
--------------

```yml
git_clone_system_user: "git-clone"     # A user that will own the cloned directory 
git_clone_system_group: "www-data"     # The group name that owns the cloned directory
git_clone_shell: "/bin/bash"     # The system user shell
git_clone_dest_path: "/tmp/tmp"     # The desired path for the cloned repository
git_clone_repo_url: "git@github.com:onaio/floip-canopy.git"   # The git repository URL(SSH)
git_clone_repo_version: master   # A branch, tag or commit hash to use when cloning
git_clone_handler_names:   # List of handlers to be notified by the role
```

Testing
-------

This role uses molecule for testing. To test, run:

    $ molecule test

License
-------

Apache 2.0

Authors
------------------

[Ona Engineering](https://ona.io)
