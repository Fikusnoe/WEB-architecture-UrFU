# Практическая работа №1 Основы командной строки Linux
## Создание виртуальной машины ##
![Параметры виртуальной машины в процессе создания](Screenshots/01-vm-settings.png)
![Командная строка Ubuntu после установки с приглашением](Screenshots/02-vm-console.png )
## Информация о системе ##
![Вывод cat ~/report/01-system.txt](Screenshots/03-system-info.png )
## Сеть: IP-адрес и открытые порты ##
![Вывод ip addr show](Screenshots/04-ip-addr.png)
![Вывод ip addr show](Screenshots/05-ports.png)
## Сервис SSH ##
![Вывод sudo systemctl status ssh](Screenshots/06-ssh-status.png)
![Вывод sudo ss -tlnp | grep ssh](Screenshots/07-ssh-port.png)
## Пользователи и группы ##
![Вывод grep '/bin/bash' /etc/passwd](Screenshots/08-users.png)
![Процесс создания пользователя boardy](Screenshots/09-new-user.png)
![Вывод id boardy](Screenshots/10-user-check.png)
## Дерево каталогов ##
![Вывод ls -la /](Screenshots/11-root-tree.png)
![Вывод ls -la ~](Screenshots/12-home-tree.png)
## Права доступа ##
![Вывод ls -ld / /etc /var /tmp /home](Screenshots/13-permissions.png)
![Три состояния testfile.txt (до, после chmod 755, после chmod 600)](Screenshots/14-chmod.png)
## Установленные пакеты и сервисы ##
![Вывод dpkg -l | grep -E 'openssh|python|git|curl|vim|nano'](Screenshots/15-packages.png)
![Вывод systemctl list-units --type=service --state=running](Screenshots/16-services.png)
## Конвейер и перенаправление ##
![Вывод ps aux --sort=-%mem | head -11](Screenshots/17-top-processes.png)
![Вывод ps aux --sort=-%mem | head -11](Screenshots/18-process-count.png)
![Вывод топ-10 больших файлов в /var](Screenshots/19-big-files.png)
## Итоговый файл ##
![Вывод ls -lh ~/report/ со всеми файлами](Screenshots/20-report-files.png)
