# Инструкция по пользованию системой git(разработано и выполнено Фабрициус А.В.)
## Topic 1: Общее назначение 
**Контроль версий (контроль исходного кода)** — практика, которая позволяет отслеживать
изменения исходного кода и управлять ими. Таким образом, *система контроля* — это реализованная возможность замены информации 
с использованием сохраненных версий.

*Основное применение* включает в себя функции:
1. хранения разных версий проекта;
2. возвращения состояния этих версих;
3. контроль нескольких ветвей состояни;
4. комментирования отдельных состояний.

## Использование системы git. Что такое GitHub?


![Перечень основных команд по использованию системы git](https://robotrackkursk.ru/wp-content/uploads/7/b/7/7b70c59517ca4da351b1f4822e35c90e.png)
### Работа Pull request
In next topic, we will talking about *pull request*. There could add some changing into a git project of your teammates\friends\colleges. If you need it, thereby you chould download your code by this. Below we explain the algoritm.
1. Check your repository on GitHub. Look for worked branch and click the button **Pull request**(all commits and differences that add into *request*, showed on the screen );
2. You see the app of chosing of basic or original version. on the left side, you see a relative repository, into this you add your changes. On the right side, you see you basic repository, from this one you pull yor commits with special ID.
3. When you finish and review at all. You click *send pull request*
4. After last 3 topics, you just will have to wait and check your request, check what will write a maintaner.
### Более подробно о commit
Основы работы с Git предполагают понимание коммитов. Команда git commit откроет текстовый редактор для ввода сообщения коммита. Также эта команда принимает несколько аргументов:

- -m позволяет написать сообщение вместе с командой, не открывая редактор. Например git commit -m "Пофиксил баг";
- -a переносит все отслеживаемые файлы в область подготовленных файлов и включает их в коммит (позволяет пропустить git add перед коммитом);
- --amend заменяет последний коммит новым изменённым коммитом, что бывает полезно, если вы неправильно набрали сообщение последнего коммита или забыли включить в него какие-то файлы.
Советы для эффективного введения в Git:

Коммитьте как можно чаще.
Одно изменение — один коммит: не помещайте все не связанные между собой изменения в один коммит, разделите их, чтобы было проще откатиться.
Формат сообщений: заголовок должен быть в повелительном наклонении, меньше 50 символов в длину и должен логически дополнять фразу this commit will ___(this commit will fix bugs — этот коммит исправит баги). Сообщение должно пояснять, почему был сделан коммит, а сам коммит показывает, что изменилось.
Если у вас много незначительных изменений, хорошим тоном считается делать небольшие коммиты при разработке, а при добавлении в большой репозиторий объединять их в один коммит.
История коммитов в Git

Коммиты хранят состояние файловой системы в определённый момент времени и указатели на предыдущие коммиты. Каждый коммит содержит уникальную контрольную сумму — идентификатор, который Git использует, чтобы ссылаться на коммит. Чтобы отслеживать историю, Git хранит указатель HEAD, который указывает на первый коммит (мы следуем по цепочке коммитов в обратном порядке, чтобы попасть к предыдущим коммитам).

Мы можем ссылаться на коммит либо через его контрольную сумму, либо через его позицию относительно HEAD, например HEAD~4 ссылается на коммит, который находится 4 коммитами ранее HEAD.

---
**GitHub** - Сервис компании Майкрософт для
организации работы удаленных
репозиториев  
Как настроить совместную работу
Углубляемся в контроль версий | Лекция 3
1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. 

 GitHub при создании нового репозитория подскажет, как это можно сделать

4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно, 
вам нужно будет авторизоваться на удалённом репозитории
5. Провести изменения “с другого компьютера”
6. Выкачать (pull) актуальное состояние из удалённого репозитория
 
### Немного подробнее о git в источниках:
[Краткое (неофициальное) руководство по работе](https://proglib.io/p/git-for-half-an-hour)

[Официальный manual по git](https://git-scm.com/docs/user-manual)

[Официальный manual по github](https://github.com/git-guides)


    Some instruction about working with directories. In a way to copy your repository from GitHub you can use `git clone` to transmit your file tgi
        When you start working with branche and you want merge one within another, you should change a branch to ones that you want to merge with.
<<<<<<< HEAD
    Notice: then you switch branch to one another, you may lost commits from another branches, if you didn, but you must
=======
    Notice: then you switch branch to one another, you may lost commits from another branches, if you didn, but you should
>>>>>>> main3
