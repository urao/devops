
### Helpful notes

```
ansible-config dump
ansible-doc --list
ansible-playbook -i inventory/ debug.yml --syntax-check 
ansible-playbook -i inventory/ debug.yml --ask-pass
find . -name '*.yml' | xargs yamllint -s
```

```
mkdir -p group_vars host_vars library module_utils filter_plugins
mkdir -p roles/common/{tasks,handlers,templates,files,vars,defaults,\
                       meta,library,module_utils,lookup_plugins}
touch production staging site.yml roles/common/{tasks,handlers,templates, \
                       files,vars,defaults,meta}/main.yml
```

End a play
```
- meta: end_play
- fail:
```

Run playbook from a docker container
```
ansible-playbook -i 192.168.0.190, -u root -e "@./newhost.json" -v simple_pb.yml
docker run -it <container_name> update_dhcpd_conf.yml -i 192.168.0.190, -e "@./newhost.json"
```

## References
[Ansible CheatSheet](https://gist.github.com/AdamOssenford/344ffe76db0a52e9051a)
