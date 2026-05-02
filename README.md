# Ansible playbook для настройки Linux сервера

## Описание
Playbook устанавливает и настраивает nginx и базовые утилиты на Ubuntu сервере.

## Требования
- Ansible 2.9+
- SSH доступ к серверу

## Установка и запуск

# Клонировать репозиторий
git clone https://github.com/egorch1/ansible_server_setup.git
cd ansible_server_setup

# Скопировать и настроить инвентарь
cp inventory.example.yaml inventory.yaml
# Заменить YOUR_SERVER_IP на IP вашего сервера

# Запустить плейбук
ansible-playbook -i inventory.yaml setup.yml
## CI/CD

Проект использует GitHub Actions для автоматической проверки:

- **Синтаксис Ansible** — проверка при каждом push
- **Линтинг** — анализ качества кода
