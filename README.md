Запуск генерации виртуальных машин для поднятия серверов через Vagrant:

```
vagrant up
```

Запуск плейбука командой:

```
ansible-playbook -i inventory all.playbook.yml --vault-password-file=.pass
```

где .pass - файл с Vault паролем (123)

Для запуска по тегам использовать:

```
--tag "<название роли>"
```

Можно использовать массив тегов

```
--tag "<название роли 1>, <название роли 2>"
```
