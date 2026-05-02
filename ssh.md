---
# Activez ssh
---
```
# Dans Termux
pkg install openssh
sshd
```

- Par défaut sshd sur Termux écoute sur le port 8022
```
# Dans Kali
ssh juesp311@100.83.233.61 -p 8022
```

---
## Pour le mot de passe, soit tu en définis un dans Termux avec passwd, soit tu copies ta clé SSH :
---

```
# Depuis Kali, copier ta clé
ssh-copy-id -p 8022 juesp311@100.83.233.61
```
> Résultat
```
/go/kaido-web/sql $ psql -d kaido_db -f ~/go/kaido-web/sql/schema.sql
psql:/data/data/com.termux/files/home/go/kaido-web/sql/schema.sql:6: NOTICE:  relation "conversations" already exists, skipping
CREATE TABLE
psql:/data/data/com.termux/files/home/go/kaido-web/sql/schema.sql:14: NOTICE:  relation "messages" already exists, skipping
CREATE TABLE
psql:/data/data/com.termux/files/home/go/kaido-web/sql/schema.sql:24: NOTICE:  relation "cron_jobs" already exists, skipping
CREATE TABLE
psql:/data/data/com.termux/files/home/go/kaido-web/sql/schema.sql:29: NOTICE:  relation "settings" already exists, skipping
CREATE TABLE
INSERT 0 0
~/go/kaido-web/sql $ cd ~/go/kaido-web
go mod init kaido-web
go get github.com/lib/pq
go: creating new go.mod: module kaido-web
go: to add module requirements and sums:
        go mod tidy
go: downloading github.com/lib/pq v1.12.3
go: added github.com/lib/pq v1.12.3

```


