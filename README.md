# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

```text
/group_vars/deb/examp.yml
```

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

```text
ansible-playbook site.yml -i inventory/test.yml
```

3. Какой командой можно зашифровать файл?

```text
ansible-vault encrypt group_vars/deb/examp.yml
```
4. Какой командой можно расшифровать файл?

```text
ansible-vault decrypt group_vars/deb/examp.yml
```
5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

```text
ansible-vault view group_vars/deb/examp.yml
```
6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

```text
ansible-playbook site.yml -i inventory/prod.yml --ask-vault-pass
```
7. Как называется модуль подключения к host на windows?

```text
winrm
```
8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

```text
ansible-doc -t connection ssh
```
9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

```text
- remote_user
        User name with which to login to the remote server, normally
        set by the remote_user keyword.
        If no user is supplied, Ansible will let the ssh client binary
        choose the user as it normally
```
