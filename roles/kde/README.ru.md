# Ansible Minimal KDE Role

<table>
<tr>
    <th>Переменная</th>
    <th>Значение по умолчанию</th>
    <th>Описание</th>
    <th>Примечание</th>
</tr>
<tr>
<td>

`managed_firewall.enabled`

</td>
<td>

`true`

</td>
<td>Отвечает за взаимодействие с брандмауэрами</td>
<td>

Если для управления брандмауэром не используется менеджеры UFW или firewall, то установите значение переменной `enabled`в `false`.

Пример:

``` yaml
managed_firewall:
  enabled: false
```
</td>
</tr>
<tr>
<td>

`kde_packages_extra: []`

</td>
<td>

`[]`

</td>
<td>Позволяет установить дополнительные пакеты через инвентарь</td>
<td></td>
</tr>
<tr>
<td>

`kde_uninstall_packages: []`

</td>
<td>

`[]`

</td>
<td>Позволяет удалить пакеты через инвентарь</td>
<td></td>
</tr>
</table>
