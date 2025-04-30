opendkim
=================

Setup OpenDKIM

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `opendkim_domains`

設定するドメイン

#### `opendkim_selector`

DKIMセレクター

#### `opendkim_packages`

インストールするパッケージ

#### `opendkim_rsa_keylen`

opendkim-genkeyで鍵を生成する時のキー長

#### `opendkim_port`

OpenDKIMのポート番号

#### `opendkim_mta`

連携させるMTA

#### `opendkim_socket`

OpenDKIMのSocket項目の設定値

#### `opendkim_cfg`

OpenDKIMの設定

#### `opendkim_trusted_hosts`

接続を許可するホストの設定

#### `opendkim_postfix_cfg`

Postfixの連携設定

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `opendkim_user`

#### `opendkim_group`

#### `opendkim_table_config_dir`

#### `opendkim_key_dir`

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: opendkim
```

License
--------------

Apache License 2.0
