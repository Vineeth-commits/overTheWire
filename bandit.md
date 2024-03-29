# Over the Wire: Bandit
---
## Level 0
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
## level 1
```bash
cat readme
```
Use the password in the file to connect to ssh
## level 2
When cat sees the string - as a filename, it treats it as a synonym for stdin. To access it -
```bash
cat ./-
```
## level 3
```bash
cat spaces\ in\ this\ filename
```
## level 4
```bash
ls -a inhere
cat .hidden
```
## level 5
```bash
file inhere/*
```
A human readable file will be of ASCII text type
## level 6
```bash 
cd inhere
find -type f -size 1033c | xargs cat
```
## level 7
```bash
find / -type f -size 33c -user bandit7 -group bandit6 2> /dev/null | xargs cat
```
## level 8
```bash
cat data.txt | grep millionth
```
## level 9
```bash
sort data.txt | uniq -u
```
## level 10
```bash
strings data.txt | grep ==
```
## level 11
```bash
sort data.txt | base64 -d
```
## level 12
```bash
sort data.txt | tr 'a-zA-Z' 'n-za-mN-ZA-M'
```
## level 13
```bash
