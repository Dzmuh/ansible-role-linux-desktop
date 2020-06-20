# Ansible Minimal Firewall Role

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

Если для управления брандмауэром не используется менеджеры UFW или firewall, то установите значение переменной `enabled`в `false`. Более того, если это не изменить, UFW или firewall будут установлены в системе.

Пример:

``` yaml
managed_firewall:
  enabled: false
```
</td>
</tr>
</tr>
</table>

## Ссылки

* [ufw – Manage firewall with UFW — Ansible Documentation](https://docs.ansible.com/ansible/latest/modules/ufw_module.html)