#Гит это легко!
---
Я потратил всего 1 час чтобы выучить основы гита, так что это легко и просто



# Шпаргалка
---

## Хеш

Если прописать комманду 'git log', то будет выведена информация о коммите, в ней будет уникальный индентификатор коммита, это и есть кеш

## Лог(Log)

После прописывания команды 'git log', мы увидим примерно такой текст:
*commit e859e4a2d470de622e63cea0471f2d626ceda5b7 (HEAD -> master, origin/master)
Author: Layne <layne.channel.official@gmail.com>
Date:   Thu May 9 12:52:13 2024 +0300

    Добавить пункт "кеш" в шпаргалку.*

В этой информации:
1. **commit** - уникальный индентификатор
2. **author** - ну тут и так понятно
3. **date** - дата создания коммита
Этой информации будет достаточно чтобы читать лог.
[Практикум](https://practicum.yandex.ru/trainer/git-basics/lesson/2e019bb7-08bf-49ed-9860-26c0bdd8fe8a/ "Тут более детальная теория")

## Статусы файлов

Файлы могут быть untraced/tracked, staged и modifed
- **untracked** - это когда гит не отслеживает изменение файла.
- **tracked** - гит уже начал отслеживать изменение файла, и как правило он уже был закомичен и добавлен командой git add
- **staged** - это состояние когда файл был добавлен командой 'git add', но не был закомичен
- **modifed** - закомиченный файл был отредактирован, но не был обновлен командой 'git commit'

```mermaid
status files
    A[untracked] -- git add --> B{staged};
    B -- git commit --> C[tracked];
    C -- изменения в файле --> D[modifed];
```
