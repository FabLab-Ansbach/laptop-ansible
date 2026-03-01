# laptop-ansible

Ansible Playbooks für die Laptops im FabLab.

Passwort für die Vaults wird in .vaultpasswd abgelegt und kann bei Kilian erfragt werden.

## Dependencies installieren

```bash
ansible-galaxy install -r requirements.yml
```

## Playbook ausführen

```bash
ansible-run setup  # Base setup
ansible-run reset  # Nutzerverzeichnis zurücksetzen
ansible-run update # Alle Pakete aktualisieren#
```

## Rollen hinzufügen

Wenn neue Rollen entwickelt werden, die ggf. in anderen Playbooks verwendet werden können (oder ggf. für andere Labs nützlich sind), sollten sie in einem eigenen Repository (`ansible-role-*`) abgelegt werden und in requirements.yml aufgenommen werden.
