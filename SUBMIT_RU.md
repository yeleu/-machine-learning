# Как открыть и сдать

SEED = 2962. Все пять частей выполнены в student2962_task2.ipynb на английском языке; результаты вычислений и график сохранены. requirements.txt содержит исходные версии курса. История Git включена в архив; коммиты сделаны ассистентом по мере подготовки, без подмены автора.

1. Распакуйте архив целиком, включая скрытую папку .git. Замените student2962 в имени папки и notebook на свою фамилию латиницей. Не меняйте SEED.
2. Откройте notebook и проверьте, что понимаете вычисления и выводы.
3. Для повторного запуска создайте окружение внутри папки проекта:

```bash
python -m venv .lastname_ML_task_2
```

Активируйте его: Windows PowerShell `.lastname_ML_task_2\Scripts\Activate.ps1`, macOS/Linux `source .lastname_ML_task_2/bin/activate`.

```bash
pip install -r requirements.txt
pip install notebook ipykernel
python -m ipykernel install --user --name ml-task2 --display-name "ML Task 2"
jupyter notebook
```

Выберите ядро ML Task 2. Выполните Restart & Run All и сохраните notebook. Jupyter намеренно не добавлен в requirements.txt, как требует задание.

4. Проверьте историю: `git log --oneline`. Не выполняйте новый git init, если .git сохранена. После переименования сохраните изменения:

```bash
git add -A
git commit -m "Set student surname and verify notebook"
```

При первом личном коммите Git может попросить ваше имя и email; задайте свои действительные данные.

5. На GitHub создайте новый пустой репозиторий без README, .gitignore и лицензии. Затем выполните (замените YOUR-USERNAME и YOUR-REPO):

```bash
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git
git push -u origin main
```

Если репозиторий приватный, добавьте преподавателя unreal-kz через Settings → Collaborators → Add people.

6. Откройте последний коммит на GitHub и скопируйте его URL вида https://github.com/YOUR-USERNAME/YOUR-REPO/commit/FULL-SHA. Именно этот URL сдаётся в Canvas, а не ZIP, notebook или адрес корня репозитория.

Срок: 9 октября 2026, 23:59 (UTC+5). Внешний репозиторий и отправка в Canvas ещё не выполнены.
