# ansible-swarm

A role for installing swarm.


## Actions

- Ensures that swarm is installed (using `apt`)


## Usage:
```
  - name: Install swarm
    hosts: swarm
    user: root
  #  connection: local

    vars_prompt:
    - name: jenkins_username
      prompt: "What is your jenkins user?"
      private: no
    - name: jenkins_password
      prompt: "What is your jenkins password?"
      private: yes

    roles:
      - swarm
```

## License

MIT
