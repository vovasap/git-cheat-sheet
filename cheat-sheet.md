# git-cheat-sheet

## Вывести список веток
#### Вывести список локальных веток

    git branch

#### Вывести список всех веток

    git branch -a

## Удаление ветки
#### Удаление локальной ветки
Удаляемая ветка не должна быть текущей веткой.

    git branch -d MyLocalBrach

или

    git branch --delete MyLocalBrach

Принудительное удаление:

    git branch -D MyLocalBrach

#### Удаление удаленной ветки

    git push origin -d MyRemoteBrach

или

    git push origin --delete MyRemoteBrach
