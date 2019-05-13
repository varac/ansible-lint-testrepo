# Ansible-lint test-repo

When I lint the playbook that includes the `configure` role, I see this warning:

    $ ansible-lint -p test.yml
    /home/varac/projects/config-management/ansible/examples/test-playbook/roles/configure/tasks/main.yml:1: [E301] Commands should not change things if nothing needs doing

But when I lint the file itself, ansible-lint doesn't warn:

    $ ansible-lint -p roles/configure/tasks/main.yml
    $
