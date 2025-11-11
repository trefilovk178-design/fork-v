Задание: Создание форка и настройка локального репозитория 🎯 Цель Освоить workflow участия в open-source проектах через создание форка и настройку локальной среды разработки.

📋 Шаги выполнения Шаг 1: Выбор репозитория Перейдите на GitHub

Найдите репозиторий: https://github.com/octocat/Spoon-Knife

Или выберите любой другой открытый проект

Шаг 2: Создание форка на GitHub На странице репозитория нажмите кнопку "Fork" (правый верхний угол)

Выберите ваш аккаунт как место для форка

Дождитесь создания копии репозитория

Шаг 3: Клонирование на локальную машину bash

Скопируйте URL вашего форка (кнопка "Code" на GitHub)
git clone https://github.com/ВАШ_АККАУНТ/Spoon-Knife.git

Перейдите в папку проекта
cd Spoon-Knife Шаг 4: Настройка связей с оригинальным репозиторием bash

Добавьте оригинальный репозиторий как upstream
git remote add upstream https://github.com/octocat/Spoon-Knife.git

Проверьте подключенные remote-репозитории
git remote -v Ожидаемый вывод:

text origin https://github.com/ВАШ_АККАУНТ/Spoon-Knife.git (fetch) origin https://github.com/ВАШ_АККАУНТ/Spoon-Knife.git (push) upstream https://github.com/octocat/Spoon-Knife.git (fetch) upstream https://github.com/octocat/Spoon-Knife.git (push) Шаг 5: Создание feature-ветки bash

Создайте новую ветку для ваших изменений
git checkout -b my-feature-branch Шаг 6: Внесение изменений Создайте файл student-info.txt

Добавьте в него:

text Имя: [Ваше имя] Дата: [Сегодняшняя дата] Уровень: Начальный Цель: Изучение Git workflow Сохраните файл

Шаг 7: Фиксация изменений bash

Добавьте файл в staging area
git add student-info.txt

Создайте коммит
git commit -m "docs: add student information file" Шаг 8: Отправка изменений в ваш форк bash

Отправьте ветку в ваш форк на GitHub
git push origin my-feature-branch Шаг 9: Синхронизация с оригинальным репозиторием bash

Вернитесь в основную ветку
git checkout main

Получите изменения из оригинального репозитория
git fetch upstream

Обновите вашу основную ветку
git merge upstream/main ✅ Проверка результатов На GitHub: В вашем аккаунте есть форк репозитория

Создана ветка my-feature-branch

Файл student-info.txt присутствует в ветке

Локально: Репозиторий склонирован на компьютер

Настроены оба remote: origin и upstream

Создана и переключена feature-ветка

Изменения закоммичены

Основная ветка синхронизирована с оригиналом

Проверка командой: bash

Проверьте историю коммитов
git log --oneline -5

Проверьте статус репозитория
git status

Проверьте ветки
git branch -a 🔄 Дополнительное задание Создание Pull Request (опционально) На GitHub перейдите в ваш форк

Нажмите "Compare & pull request"

Создайте PR из my-feature-branch в main вашего же форка

Напишите описание изменений

Завершите создание PR

📝 Итоговый результат После выполнения всех шагов у вас будет:

✅ Полностью настроенная локальная среда разработки

✅ Понимание workflow fork-based разработки

✅ Практический опыт работы с ветками и remote-репозиториями

✅ Готовность к участию в реальных open-source проектах

Время выполнения: 15-25 минут
