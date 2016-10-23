# Ansible Playbook for Rails Application

* ConohaVPSのCentOS7を対象にしたAnsibleです

## 使い方

* memoファイルの通り、SSHの初期設定を完了させる
* 変数ファイルを自身の環境に合わせる

```
cp production.default production
cp group_vars/production.yml.default group_vars/production.yml
```

* ansibleの実行

```
ansible-playbook -i production server.yml
```

* `mysql_secure_installation`は手動実行
