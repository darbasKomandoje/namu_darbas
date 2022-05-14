# Pasiruošimas darbui

Projekto nusiklonavimas:

```bash
git clone git@github.com:darbasKomandoje/namu_darbas.git
```
Prieš atlikdami pakeitimus, pasikeiskite į savo branch'ą:
```bash
git checkout -b ＜new-branch＞
```

## Atliktų pakeitimų išsaugojimas
Kuriuos redaguotus failus įtrauksite, jeigu po add nurodysite žvaigždutę, visi redaguoti failai bus įtraukti:
```bash
git add ＜index.html＞
```
Žinutė, kurioje nurodote kas buvo atlikta:
```bash
git commit -m "your text"
```
## Pakeitimų išsiuntimas į nutolosi serverį
```bash
git push <remote> <branch-name>
```

## Pasimetus, kurioje šakoje dirbate
```bash
git status
```
## Programavau ir ops... Pamačiau, kad sukomitinau pakeitimus į main šaką, ką daryti?
Vieno commito panaikinimas:
```bash
git reset HEAD~1
```
Tada naujo branch'o kūrimas ir visi pakeitimai užfiksuoti jame:
```bash
git checkout -b newbranch

git add -A

git commit -m "Committed on new branch"
```
