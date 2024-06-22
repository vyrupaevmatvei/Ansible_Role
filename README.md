Ansible Role: User Password Setup
Эта роль Ansible устанавливает пароль для пользователя и включает необходимость смены пароля при первом входе в систему.
Структура проекта

Ansible_Role/
├── defaults
│   └── main.yml          # Значения по умолчанию для переменных роли(добавить при необходимости)
├── tasks
│   └── main.yml          # Основные задачи роли
├── vars
│   └── main.yml          # Переменные роли
├── hosts.ini             # Нужные хосты
├── playbook.yaml         # Пример плейбука
├── playbook2.yaml        # Плейбук с переменными и тасками внутри
└── README.md             # Документация роли

Запустите плейбук с использованием инвентори файла:
ansible-playbook -i hosts.ini playbook.yml --ask-become-pass
