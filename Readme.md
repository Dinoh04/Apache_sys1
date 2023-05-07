# Exercice sur les commandes linux avec bandit

## Level 0

On utilise l'hôte pour se connecter à bandit, ssh bandit0@bandit.labs.overthewire.org -p 2220 le premier hôte avec mot de passe : bandit0.

## Level 1


Pour se connecter à Bandit, il faut exécuter la commande suivante :

`hôte: ssh bandit0@bandit.labs.overthewire.org -p 2220`

Une fois connecté, vous pouvez exécuter les commandes suivantes :

```bash
- `ls` pour afficher la liste des fichiers dans le répertoire courant
- `cat readme` pour afficher le contenu du fichier readme

Le mot de passe pour le niveau suivant est : NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

```
# Level 2
```bash
ls
cat ./- pour afficher le mot de passe


```
> Mot de passe pour le niveau suivant est: <span style="color:green;">rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi</span>

# Level 3
```bash
ls
cat ./ spaces +TAB	pour afficher spaces\ in\ this\ filename


```
> Mot de passe pour le niveau suivant est: <span style="color:green;">aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG</span>


# Level 4
```bash
ls
cd inhere
cat .hidden

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe</span>


# Level 5
```bash
ls 
cd inhere
cat ./-file07
```
> Mot de passe pour le niveau suivant est: <span style="color:green;">lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR</span>


# Level 6
```bash
find inhere -type f -size 1033c -not -executable -exec file {} \; | grep "ASCII text" | cut -d: -f1 | xargs cat

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU</span>


# Level 7
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat  /var/lib/dpkg/info/bandit7.password

```
> Mot de passe pour le niveau suivant est: <span style="color:green;"> z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S</span>

# Level 8
```bash
ls
data.txt
grep "millionth" data.txt

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">TESKZC0XvTetK0S9xNwm25STk5iWrBvP</span>

# Level 9
```bash
ls
sort data.text | uniq -u

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">EN632PlfYiZbn3PhVK3XOGSlNInNE00t</span>

# Level 10
```bash
ls
strings data.txt | grep "===="
```
> Mot de passe pour le niveau suivant est: <span style="color:green;">G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s</span>

# Level 11
```bash
ls
cat data.txt | base64 -d

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM</span>
# Level 12
```bash
ls
cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv</span>

# Level 13
```bash
 mkdir /tmp/newfolder
ls
cat data9

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw</span>

# Level 14
```bash
ls
cat sshkey.private
ssh -i sshkey.private bandit14@localhost  -p 2220

```
> Pour cet niveau il est tout de suite rediriger vers bandit15

# Level 15
```bash
cd /etc/bandit_pass/
cat bandit14
echo fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq | nc localhost 30000

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt</span>

# Level 16
```bash
ls
cat /etc/bandit_pass/bandit15
openssl s_client -connect localhost:30001

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">JQttfApK4SeyHwDlI9SXGR50qclOAil1</span>
# Level 17
```bash
nmap -A localhost -p 31000-32000
cat /etc/bandit_pass/bandit16
openssl s_client -connect localhost:31790
cd /tmp
nano ssh-17.private

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e</span>
# Level 18
```bash
ls
diff passwords.new passwords.old

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg</span>

# Level 19
```bash
ssh -T bandit18@bandit.labs.overthewire.org -p 2220
ls
cat readme

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">awhqfNnAbc1naukrpqDYcF95h7HoMTrC</span>

# Level 20
```bash
ls
file bandit20-do
./bandit20-do
./bandit20-do cat /etc/bandit_pass/bandit20

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">VxCazJaVykI6W36BkBU0mJTCM8rR95XT</span>
# Level 21
```bash
ls
echo -n VxCazJaVykI6W36BkBU0mJTCM8rR95XT | nc -l -p 1234 & [1] 2227708
./suconnect 1234
Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
Password matches, sending next password

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">NvEJF7oVjkddltPSrdKEFOllh9V1IBcq</span>

# Level 22
```bash
cd /etc/cron.d
ls
cat cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff</span>
# Level 23
```bash
cd /etc/cron.d
ls
cat cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
echo I am user bandit23 | md5sum | cut -d ' ' -f 1
cat /tmp/8ca319486bfbbc3663ea0fbe81326349

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G</span>

# Level 24
```bash
cd /etc/cron.d
ls
cat /usr/bin/cronjob_bandit24.sh
mkdir /tmp/kunci
chmod 777 /tmp/kunci
cd /tmp/kunci
cp shell-kunci.sh /var/spool/bandit24/
ls
cat ikikunci

```
> Mot de passe pour le niveau suivant est: <span style="color:green;">UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ</span>
