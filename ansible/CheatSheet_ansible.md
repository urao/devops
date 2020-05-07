
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

## References
[Ansible CheatSheet](https://gist.github.com/AdamOssenford/344ffe76db0a52e9051a)
