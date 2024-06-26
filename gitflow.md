# ![icons8-слияние-веток-в-git-30](https://github.com/HasanDzhabrailov/Money-Traking-/assets/51163032/b3c24bf3-422e-4208-9bb6-ba37190811b1) Git Workflow

## 📌 Специфика:
- **1 ветка = 1 задача**
- Перед созданием **Merge Request'а** необходимо обновить свою ветку, стянув для этого изменения с `developer` ветки и **локально** решить **ВСЕ** появившиеся конфликты
- Ветки, "готовые" и уже слитые в `developer`, должны быть удалены после **Merge Request'а**
- ❗ **ОБЯЗАТЕЛЬНО** пользоваться **[.gitignore](../../.gitignore)** файлами, чтобы не залить в репозиторий папку .idea и другие генерируемые файлы которые не нужны вашим коллегам, но сильно раздувающие репозиторий ❗

## 📌 Ветки:
| Тип             | Описание                                  | Примеры                    | 
|-----------------|-------------------------------------------|----------------------------|
| **feature**     | Новый функционал                          | `feature/MT-239193`     |
| **bugfix**      | Исправление ошибок                        | `bugfix/MT-191119`      |
| **improvement** | Техдолг, доработка, обновления, улучшения | `improvement/MT-107010` |
| **concept**     | Плавный переход и/или замена функционала  | `concept/MT-141151`     |


## 📌 Коммиты:
### Структура коммита:

```text
*тип ветки*/MT-*номер задачки* changes:

- Change 0  
- Изменение 1  
- Change 2  
- Изменение  3  
```
Такая структура коммита позволяет иметь читабельное описание в виде выпадающего списка в **GitHub**, понимать на какой ветке существует этот коммит, быстро находить задачу привязанную к этим изменениям, а так же иметь общее представление по типу ветки о содержании изменений.
#### Пример коммита:
```text
feature/MT-239193 changes:

- Добавлен дизайн главного экрана
- Добавлен дизайн авторизации
- Вырезано старое меню
```

## 📌 Pull Request 
### **Пример:**
**✏️ Title**  (название ветки + заголовок задачки)
```
improvement/MT-239193 Описание Readme
```  

**✏️ Описание** (Все пункты с изменениями из всех коммитов ветки)  
```- Файл README.md дополнен правилами git workflow 
- Добавлено описание клонирования и запуска проекта
- Добавлено описание архитекутры проекта
```
**🎯 Merge options**

✅ `Rebase and merge`  

❗ Так же указываем себя в поле `Assignee` и  HasanDzhabrailov в `Reviewer` ❗
