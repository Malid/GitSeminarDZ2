# Команды GIT
1. **git config --global user.name "Name"** - set or change the username to display in git.
2. **git config --global user.email "myemail@mail.com"** set or change the email address recorded in git
3. **git init** - repository initialization
4. **git status** - check repository status
5. **git add filname.ext** или **git add .** -adding individual files or all files to the staged files area
6. **git commit -m "Message About Commit"** - creating a commit
7. **git log** - view commit history with changes
8. **git diff** - view changes before commit
9. **git checkout _<BranchName или первые символы хеша коммита>_** - переход в указанную ветку или коммит
10. **git checkout -b new_branch_name** - создание новой ветки и переход в неё
11. **git branch new_branch_name** - создание новой ветки
13. **git branch** - просмотр списка веток
14. **git branch -d branch_to_delete** - удаление ветки так чтобы ничего не сломать
15. **git merge branch_name** - Объединение указанной ветки с основной
16. **git log --graph** - Отображение журнала веток в виде графика

*если в репозитории создать файл **.gitignore** и добавить туда список файлов, например картинок или больших файлов, при добавлении файла **.gitignore** в репозиторий, git не будет обрабатывать эти файлы

**git log -n** Отобразить последние n коммитов

**git log --since 2022-01-17 _until 2022-01-22_** отобразить коммиты с определенной даты *по определённую дату (необязательно)*