# GIT commands
1. **git config --global user.name "Name"** - set or change the username to display in git.
2. **git config --global user.email "myemail@mail.com"** set or change the email address recorded in git
3. **git init** - initialization of the repository
4. **git status** - check the status of the repository
5. **git add filname.ext** or **git add .** - add individual files or all files to the staging area
6. **git commit -m "Message About Commit"** - create a commit
7. **git log** - view commit history with changes
8. **git diff** - view changes before commit
9. **git checkout _<BranchName or the first characters of the commit hash>_** - jump to the specified branch or commit
10. **git checkout -b new_branch_name** - create a new branch and switch to it
11. **git branch new_branch_name** - create a new branch
13. **git branch** - view list of branches
14. **git branch -d branch_to_delete** - delete a branch without breaking anything
15. **git merge branch_name** - Merging the specified branch with the current one
16. **git log --graph** - Display branch log as a graph

*если в репозитории создать файл **.gitignore** и добавить туда список файлов, например картинок или больших файлов, при добавлении файла **.gitignore** в репозиторий, git не будет обрабатывать эти файлы

**git log -n** Отобразить последние n коммитов

**git log --since 2022-01-17 _until 2022-01-22_** отобразить коммиты с определенной даты *по определённую дату (необязательно)*

**git rm _FileName_** удалить файл из индексов git

**git rebase main** копирует набор коммитов и переносит их в другое место

**git detaching HEAD** отделение HEAD от ветки к коммиту

**git checkout main^** переключение на уровень выше

**git checkout main~3** перемещение на 3 коммита назад

**git branch -f main HEAD~3** принудительно переместить ветку main на 3 родителя назад от HEAD


***
# Отправка локального репозитория на сервер GitHub

**git remote add origin <_WebPatch.git_>**

**git branch -M main**

**git push -u origin main**

**git push** отправить изменения на GitHub (_ТРЕБУЕТ АВТОРИЗАЦИИ_)

**git pull** загрузить с сервера. Пытается делать merge

**?git fetch** синхронизация локальной ветки с удалённой. Git pull вызывает git fetch следом за git merge
***
# Git pull request

- Делаем **fork** (ответвление) репозитория
- Делаем git clone **своей** версии репозитория
- Создаем новую ветку и в **неё** вносим свои изменения
- Фиксируем изменения (делаем коммиты)
- Отправляем свою версию в свой GitHub
- На сайте GitHub нажимаем кнопку **pull request**
***