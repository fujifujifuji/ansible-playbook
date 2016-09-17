# 使い方

hostnameを**ansible-serv**にしてあるのでコマンドの**ansible-serv**は適宜自分のhostnameに置き換えてください

## configに追加

```
vi ~/.ssh/config
```


```
Host ansible-serv
  HostName XXX.XXX.XXX.XX
  User user_name
  IdentityFile ~/.ssh/id_rsa
```

##ping確認コマンド

```
ansible ansible-serv -m ping
```

##tasks実行

```
ansible-playbook main.yml --ask-sudo-pass
```
