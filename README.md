# Домашнее задание к занятию 4 «Работа с roles» - Пугач Евгений.


---

## `Подготовка к выполнению`

Виртуальные машины `clickhouse`, `vector` и `lighthouse` разворачиваются в Yandex Cloud при помощи Terraform:

![Скриншот 1](https://github.com/PugachEV72/Images/blob/master/2023-11-25_12-12-52.png)

[TERRAFORM](https://github.com/PugachEV72/08-ansible-04-roles/tree/main/terraform_vms) 

---

## `Основная часть`

1. Создайте в старой версии playbook файл `requirements.yml` и заполните его содержимым:
```
---
  - src: git@github.com:AlexeySetevoi/ansible-clickhouse.git
    scm: git
    version: "1.13"
    name: clickhouse 
```
2. При помощи ansible-galaxy скачайте себе эту роль.
3. Создайте новый каталог с ролью при помощи ansible-galaxy role init vector-role.
4. На основе tasks из старого playbook заполните новую role. 
5. Перенесите нужные шаблоны конфигов в templates.
6. Опишите в README.md обе роли и их параметры. 
7. Повторите шаги 3–6 для LightHouse. 

### Ответ:

![Скриншот 2](https://github.com/PugachEV72/Images/blob/master/2023-11-25_12-22-39.png)

![Скриншот 3](https://github.com/PugachEV72/Images/blob/master/2023-11-25_12-24-13.png)

![Скриншот 4](https://github.com/PugachEV72/Images/blob/master/2023-11-25_12-26-05.png)

![Скриншот 5](https://github.com/PugachEV72/Images/blob/master/2023-11-25_12-28-35.png)

---

8. Выложите все roles в репозитории. Проставьте теги, используя семантическую нумерацию.  
Добавьте roles в `requirements.yml` в playbook.

### Ответ:

[VECTOR-ROLE](https://github.com/PugachEV72/vector-role)

[LIGHTHOUSE-ROLE](https://github.com/PugachEV72/lighthouse-role)

![Скриншот 6](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-18-39.png)

---

9. Переработайте playbook на использование roles. Не забудьте про зависимости LightHouse и  
возможности совмещения roles с tasks.

### Ответ:

![Скриншот 7](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-19-13.png)

---

10. Выложите playbook в репозиторий.

### Ответ:

[PLAYBOOK](https://github.com/PugachEV72/08-ansible-04-role/tree/main/playbook)

![Скриншот 8](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-15-02.png)

![Скриншот 9](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-17-44.png)

![Скриншот 10](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-18-03.png)

![Скриншот 11](https://github.com/PugachEV72/Images/blob/master/2023-11-25_18-20-13.png)

---
---




