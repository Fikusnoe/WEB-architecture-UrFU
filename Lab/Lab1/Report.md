# Практическая работа №1 Основы командной строки Linux
## 1. Создание виртуальной машины ##
1. Параметры виртуальной машины в процессе создания
![Параметры виртуальной машины в процессе создания](Screenshots/01-vm-settings.png)
2. Командная строка Ubuntu после установки с приглашением
![Командная строка Ubuntu после установки с приглашением](Screenshots/02-vm-console.png )
## 2. Информация о системе ##
1. Вывод cat ~/report/01-system.txt
![Вывод cat ~/report/01-system.txt](Screenshots/03-system-info.png )
## 3. Сеть: IP-адрес и открытые порты ##
1. Вывод ip addr show
![Вывод ip addr show](Screenshots/04-ip-addr.png)
2. Вывод sudo ss -tlnp
![Вывод sudo ss -tlnp](Screenshots/05-ports.png)
## 4. Сервис SSH ##
1. Вывод sudo systemctl status ssh
![Вывод sudo systemctl status ssh](Screenshots/06-ssh-status.png)
2. Вывод sudo ss -tlnp | grep ssh
![Вывод sudo ss -tlnp | grep ssh](Screenshots/07-ssh-port.png)
## 5. Пользователи и группы ##
1. Вывод grep '/bin/bash' /etc/passwd
![Вывод grep '/bin/bash' /etc/passwd](Screenshots/08-users.png)
2. Процесс создания пользователя boardy
![Процесс создания пользователя boardy](Screenshots/09-new-user.png)
3. Вывод id boardy
![Вывод id boardy](Screenshots/10-user-check.png)
## 6. Дерево каталогов ##
1. Вывод ls -la /
![Вывод ls -la /](Screenshots/11-root-tree.png)
2. Вывод ls -la ~
![Вывод ls -la ~](Screenshots/12-home-tree.png)
## 7. Права доступа ##
1. Вывод ls -ld / /etc /var /tmp /home
![Вывод ls -ld / /etc /var /tmp /home](Screenshots/13-permissions.png)
2. Три состояния testfile.txt (до, после chmod 755, после chmod 600)
![Три состояния testfile.txt (до, после chmod 755, после chmod 600)](Screenshots/14-chmod.png)
## 8. Установленные пакеты и сервисы ##
1. Вывод dpkg -l | grep -E 'openssh|python|git|curl|vim|nano'
![Вывод dpkg -l | grep -E 'openssh|python|git|curl|vim|nano'](Screenshots/15-packages.png)
2. Вывод systemctl list-units --type=service --state=running
![Вывод systemctl list-units --type=service --state=running](Screenshots/16-services.png)
## 9. Конвейер и перенаправление ##
1. Вывод ps aux --sort=-%mem | head -11
![Вывод ps aux --sort=-%mem | head -11](Screenshots/17-top-processes.png)
2. Вывод подсчёта процессов по пользователям
![Вывод подсчёта процессов по пользователям](Screenshots/18-process-count.png)
3. Вывод топ-10 больших файлов в /var
![Вывод топ-10 больших файлов в /var](Screenshots/19-big-files.png)
## 10. Итоговый файл ##
1. Вывод ls -lh ~/report/ со всеми файлами
![Вывод ls -lh ~/report/ со всеми файлами](Screenshots/20-report-files.png)
