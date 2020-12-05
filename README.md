# moscow-time-ansible

This is a playbook that provides `moscow-time` web app to a Linux server of choice, it installs docker and docker-compose alongside. Also, it's intended to allow for https traffic, if you pass `do_cerbot=true`.
Like that

```bash
ansible-playbook -i root@int1.tst.iroha.tech, playbook.yml -v
```

Or like that, if you want to issue certificates

```bash
ansible-playbook -i root@int1.tst.iroha.tech, playbook.yml --extra-vars 'do_certbot=true'
```

P.S. I didn't manage to finish cert bot on time and so I have this branch, but you can always look into `master` if you wish