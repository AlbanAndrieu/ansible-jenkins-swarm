ansible-jenkins-swarm
==============

A role for installing jenkins swarm.

[![Build Status](https://api.travis-ci.org/AlbanAndrieu/ansible-jenkins-swarm.png?branch=master)](https://travis-ci.org/AlbanAndrieu/ansible-jenkins-swarm)

## Actions

- Ensures that swarm is installed (using `apt`)

Usage example
------------
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
      - jenkins-swarm
```

Requirements
------------

none

Dependencies
------------

https://github.com/AlbanAndrieu/ansible-jenkins-slave

License
-------

MIT

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/AlbanAndrieu/ansible-jenkins-swarm/issues)!
