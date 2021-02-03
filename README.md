
## Именование
#### Изменить имя ветки
Изменить имя текущей ветки

    git branch -m NewName
    
Изменить имя произвольной ветки

    git branch -m OldName NewName


## Ветвление
#### Создать новую ветку

    git checkout -b NewBranch
    
Тоже самое что и

    git branch NewBranch
    git checkout NewBranch

#### Слить ветку
Переключиться на ветку, в которую нужно добавить изменения:

    git checkout TargetBranch

Добавляем изменения из ветки-источника:

    git merge SourceBranch

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

## Размещение на github pages
Источником публикации будет директория `dist` 

    git subtree push --prefix dist origin gh-pages
