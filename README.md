# lab3
# 2. Практическая часть 
# 2.1. Управление пользователями 
# 2.1.1. Создание нового пользователя
![src1](https://github.com/user-attachments/assets/0fad3c75-2b5f-43b5-9883-d080541ad5f2)
# 2.1.2. Изменение пароля пользователя 
![src1](https://github.com/user-attachments/assets/291ad50a-b025-43af-8c17-b5a3270bacf9)
# 2.1.3. Изменение интерпретатора командной строки 
![src1](https://github.com/user-attachments/assets/138b4f0f-ba7f-440a-8234-78561a238d0b)
# 2.1.4. Установка non-login shell 
![src1](https://github.com/user-attachments/assets/5b8e3415-d803-4024-9257-52278e4b118c)
# 2.1.5. Удаление пользователя 
![src1](https://github.com/user-attachments/assets/2c00c507-85f5-49fb-9a2d-af0b3034b924)
# 2.2. Управление правами доступа к файлам 
# 2.2.1. Изменение владельца файла 
![src1](https://github.com/user-attachments/assets/b4ec0445-ac12-4402-b6c1-fb2ff9e11517)
# 2.2.2. Изменение прав доступа
![src1](https://github.com/user-attachments/assets/e649ee30-4fe1-4ebb-ac52-84a2b737bade)
# 2.2.3. Специальные биты
![src1](https://github.com/user-attachments/assets/d4f75266-4c3b-45ff-81f2-9e8cf3a0a316)
# 2.3  Персонализация консоли через .bashrc
# 2.3.1. Настройка приглашения командной строки 
![src1](https://github.com/user-attachments/assets/078ea984-f600-4761-9d81-de5a08b2cd79)
# 2.3.2 Полезные алиасы 
![src1](https://github.com/user-attachments/assets/ce19734c-8d67-49df-a99b-2a6f4b25d449)
# 2.3.3 Настройка истории команд
![src1](https://github.com/user-attachments/assets/6bbfd75a-40bf-467a-b69f-032fe9baeeeb)
# 2.3.4
![src1](https://github.com/user-attachments/assets/e448390a-e265-47bf-907f-a63eb936f64f)
# 2.4.
# 2.4.1
![src1](https://github.com/user-attachments/assets/779e7e98-451b-4284-b4ca-cea9f0baef6c)
# 2.4.2 Доступные цветовые схемы 
![src1](https://github.com/user-attachments/assets/ed870912-3946-4fb3-b464-091405636d94)
# 2.4.3
![src1](https://github.com/user-attachments/assets/2aa90608-91b6-473f-9c1d-06c69260a0df)
![src1](https://github.com/user-attachments/assets/8a518f5e-9df1-4d9c-b250-fc492d32eb48)
# 5 Контрольные вопросы
# 1 Какой формат имеет файл /etc/passwd? Объясните назначение каждого поля.
Имя пользователя, зашифрованный пароль, UID, GID, настоящее имя, домашний каталог, оболочка
# 2 Чем отличаются команды useradd и adduser? Какая из них предпочтительнее для начинающих администраторов?
useradd мощнее, adduser проще для новичков.
# 3 Какие значения shell используются для non-login пользователей? В чем разница между /sbin/nologin и /bin/false?
/sbin/nologin (запрещает вход), /bin/false (всегда ошибка).
# 4 Опишите алгоритм безопасного изменения shell пользователя в файле /etc/passwd. Почему нельзя использовать обычный текстовый редактор?
Использовать usermod, редактировать через visudo.
# 5 Какие права доступа соответствуют числовым значениям 644, 755, 700? Расшифруйте каждое.
644: -rw-r--r--, 755: -rwxr-xr-x, 700: -rwx------
# 6 В чем разница между командами chown и chgrp?
chown меняет владельца, chgrp меняет группу.
# 7 Что такое SUID, SGID и Sticky bit? Приведите примеры их практического применения.
SUID: выполнение с правами владельца, SGID: с правами группы, Sticky: защита директорий.
# 8 Как применить изменения в файле .bashrc без перезагрузки системы? 
source .bashrc.
# 9 Объясните назначение переменной PS1. Какие специальные символы используются для отображения текущего каталога, имени пользователя и имени хоста?
\w (каталог), \u (пользователь), \h (хост).
# 10 Перечислите основные настройки, которые можно задать в файле ~/.vimrc для повышения удобства работы системного администратора.
set number, syntax on, tabstop=4, expandtab.
# 11 Как удалить пользователя вместе с его домашним каталогом и почтовым ящиком?
userdel -r.
# 12 Какие требования предъявляются к паролям пользователей в современных дистрибутивах Linux?
Длина не менее 8 символов, сложность, запрет словарных слов.
