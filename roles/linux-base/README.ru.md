# Ansible Minimal Base System Role

Это маленькая роль Ansible устанавливает минимальный набор пакетов.

Роль также позволяет установить дополнительные пакеты, или удалить имеющиеся, используя переменную `linux_base_packages_extra`. Пример:

``` yaml
linux_base_packages_extra:
  - { state: "absent", name: "python3-apt" }
  - { state: "latest", name: "python3-dev" }
```
В примере выше был установлен пакет `python3-dev` и удалён пакет `python3-apt`.

Для расширенного удаления пакетов используйте переменную `linux_base_uninstall_packages`. Пока этот функционал доступен только для Ubuntu. Пример:

``` yaml
linux_base_uninstall_packages:
  - rpcbind
```

Фишка этого списка, если он будет задействован, в том, что для пакетов будет задействован `purge` и `autoremove`.

## Теги

Роль предоставляет на всей процедуре выполнения тег `bootstrap` который стоит использовать при первичной настройке системы.
