# Some info about tasks usage
Generally i have creaetd roles to use it multiple times but also good way is use tasks. You can import task to your main playbook using similar code like following one:

```yaml
    ---
    - name: Run tasks code
      hosts: localhost
      become: true

      handlers:
        - name: Include handlers.
          ansible.builtin.import_tasks: tasks/handlers.yaml
      
      tasks:
        - name: Setup docker
          ansible.builtin.import_tasks:  tasks/docker.yaml

```