# ИНЦИДЕНТ №[1]:[Отсутствие gitignore.] 
## СИМПТОМ:
При развёртывании проекта догружаются расширения, которые должны быть скрыты.
## ПРИЧИНА:
При первичном осмотре кода выяснился факт отсутствия gitignore.
## РЕШЕНИЕ:
Добавление gitignore, и его заполнение
## КОММИТ:
6bc09bf0a6a55b7b7ea95a5711d2efed031eb61f
---
# ИНЦИДЕНТ №[2]:[Отсутствие расширений.] 
## СИМПТОМ:
Следуя инструкции запуска появляется ошибка:
```bash
MediTrack net8.0-windows сбой с ошибками (5) и предупреждениями (1) (3,5 с)
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(15,24): error CS0103: Имя "DotNetEnv" не существует в текущем контексте.
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(16,24): error CS0103: Имя "DotNetEnv" не существует в текущем контексте.
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(17,22): error CS0103: Имя "DotNetEnv" не существует в текущем контексте.
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(18,24): error CS0103: Имя "DotNetEnv" не существует в текущем контексте.
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(19,24): error CS0103: Имя "DotNetEnv" не существует в текущем контексте.
    C:\Users\student\source\repos\RPO_Module_Exam_c-\DatabaseService.cs(37,30): warning CS0168: Переменная "ex" объявлена, но ни разу не использована.
Сборка сбой с ошибками (5) и предупреждениями (1) через 4,6 с
```
## ПРИЧИНА:
В ходе анализа кода обнаружилось отсутствие необходимых DotNetEnv расширений.
## РЕШЕНИЕ:
В консоль диспетчера пакетов ввести команду: ``dotnet add package DotNetEnv`` для установки расширения.
## КОММИТ:
bd4084a089753fc70489a060fedad3ccc027fc94
---
