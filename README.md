# GitLab Runner with DinD (Dokploy Template)

[![Deploy with Dokploy](https://img.shields.io/badge/Deploy_with-Dokploy-black)](https://dealenx.github.io/Dokployfile/dealenx/docker-compose-gitlab-runner-dokployfile)

This template allows you to quickly deploy a GitLab Runner with Docker-in-Docker (DinD) support via Dokploy.

[English](#english) | [Русский](#русский)

---

## English

### Description
This template automatically deploys a GitLab Runner with a DinD (Docker-in-Docker) sidecar service, enabling CI/CD jobs that need to build Docker images or run containers.

### How to use
1. Go to Dokploy and create a new application from a template.
2. Provide the URL of this repository.
3. Fill in the variables:
   - **Runner Name**: Your runner's name (will be visible in GitLab).
   - **GitLab URL**: Your GitLab instance URL (e.g., `https://gitlab.com/`).
   - **Registration Token**: The runner authentication token.
   - **Concurrent Tasks**: Maximum number of simultaneous jobs.

### Where to get the token?
1. Go to your GitLab project or group.
2. Open **Settings** -> **CI/CD** -> **Runners**.
3. Click **New project runner** (or use an existing one).
4. After creation, you will see "Step 1" with a registration command. You only need the token itself (usually starts with `glrt-`).
5. Paste this token into the **Registration Token** field in Dokploy.

---

## Русский

### Описание
Шаблон автоматически разворачивает GitLab Runner и вспомогательный сервис DinD, что позволяет выполнять CI/CD задачи, требующие сборки Docker-образов или запуска контейнеров.

### Как использовать
1. Перейдите в Dokploy и выберите создание нового приложения из шаблона.
2. Укажите URL этого репозитория.
3. Заполните переменные:
   - **Runner Name**: Имя вашего раннера (отобразится в GitLab).
   - **GitLab URL**: URL вашего инстанса (например, `https://gitlab.com/`).
   - **Registration Token**: Токен аутентификации раннера.
   - **Concurrent Tasks**: Максимальное количество одновременно выполняемых задач.

### Где взять токен?
1. Перейдите в ваш проект или группу в GitLab.
2. Откройте **Settings** -> **CI/CD** -> **Runners**.
3. Нажмите **New project runner** (или используйте существующий).
4. После создания вы увидите "Step 1" с командой регистрации. Вам нужен только сам токен (обычно начинается на `glrt-`).
5. Вставьте этот токен в поле **Registration Token** в Dokploy.
