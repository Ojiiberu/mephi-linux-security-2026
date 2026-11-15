M265199

# mephi-linux-security-2026

Файл shadow очищен от хешей реальных пользователей; сохранена строка user1 и системные учётки без пароля.

| Раздел | Что сделано | Файл |
|---|---|---|
| 1 | Пользователь user1 (UID 1234), группа students, смена пароля каждые 90 дней | passwd, shadow, group |
| 2.1 | Поиск файлов с битом SUID | suid_files.out |
| 2.2 | Процессы с EUID=0 и обычным RUID | procs_euid0.out |
| 3 | set-UID на копии cat | stat.out |
| 4 | capabilities (cap_chown) на копии chown | getcap.out, stat.out |
| 5 | sudo: user1 может менять время | sudoers |
| 6 | Скриншот и история команд | mephi-screenshot.png, history.out |
