# Тестовый проект для GitHub

Создан AlexD для тренировки навыков работы с **Git** и *GitHub*.

[Курс](https://practicum.yandex.ru "Яндекс практикум")

## Теория

**~** - домашняя директория

**Коммит** - фиксация состояния в Git.

**Git** - консольный инструмент для работы с локальными и удаленными репозиториями. Проект с откртым исходным кодом.

**GitHub** - платформа для размещения удаленных репозиториев.

**Сетевые протоколы** - правила обмена данными между компьютерами.

**SSH** - сетевой протокол с шифрованием.

**SSH-пара** - приватный и публичный ключи.

**Ветка** - временная шкала, на которой расположены коммиты. Ветка всегда начинается от одного из коммитов.

Самая первая ветка в репозитории появляется автоматически и называется *main* или *master*.

**Markdowm (маркдаун)** - специальный язык разметки текстовых документов.

## Команды

```bash
git init
```

*Сделать папку репозитория (инициализировать репозиторий).*

---

```bash
git status
```

*Проверить состояние репозитория.*

---

```bash
touch
```

*Создать файл.*

---

```bash
mkdir
```

*Создать папку.*

```bash
ssh -vT git@github.com
```

*Проверка правильности ключа. Флаг **-v** - это расширенный вывод информации по процессу подключения*.

---

```bash
ssh-kegen -t ed25519 -C "email на GitHub"
```

*Создать SSH-пару.*

---

```bash
git remote add
```

*Привязать удаленный репозиторий к локальному.*

---

```bash
git remote -v
```

*Убедиться, что репозитории связаны.*

---

```bash
git remote add origin адрес_для_подключения
```

*origin - стандартный псевдоним, с помощью которого можно обратиться к главному удаленному репозиторию.*

---

```bash
git push
```

*Отправить изменения на удаленный репозиторий. В первый раз используем флаг -u для связи локального и удаленного репозиторий. Пример:*

```bash
git push -u origin master
```

## Хэш

**Хэш коммита** -  результат хэширования информации о коммите: когда был сделан коммит, содержание файлов, ссылка на предыдущий коммит. Это основной идентификатор коммита.

*Основные правила*

1. Если хэш получить дважды для одного и того же набора входных данных, то результат будет гарантированно одинаковый.

2. Если хоть что-то в исходных данных поменяется, то хеш тоже изменится.

## Log

Есть сокращенная версия команды log:

```bash
git log --oneline
```

*Позволяет получить сокращенный лог, где будет указано ровно столько символов хэша, сколько нужно для его идентификации*

## HEAD

**Файл HEAD** - указывает на коммит, который сделан последним (в нем содержится ссылка на послдений коммит). Это, своего рода, синоним хеша последнего коммита.