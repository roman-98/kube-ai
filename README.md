# Kubernetes Manifests

Цей репозиторій містить різні Kubernetes маніфести для різних сценаріїв використання. Нижче представлена таблиця з описом кожного маніфесту.

| NAME                   | PROMPT                    | DESCRIPTION                                                  | EXAMPLE                                   |
|------------------------|---------------------------|--------------------------------------------------------------|-------------------------------------------|
| app.yaml               | create deploy myapp --image=myapp:latest                | Основний маніфест для розгортання додатку.                   | [app.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app.yaml)                 |
| app-livenessProbe.yaml | create deploy myapp --image=myapp:latest --liveness-probe            | Маніфест з налаштуванням liveness probe для додатку.         | [app-livenessProbe.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml| create deploy myapp --image=myapp:latest --readiness-probe           | Маніфест з налаштуванням readiness probe для додатку.        | [app-readinessProbe.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml  | create deploy myapp --image=myapp:latest --volume-mounts             | Маніфест з налаштуванням підключення томів.                  | [app-volumeMounts.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml       | create cronjob mycronjob --schedule='*/5 * * * *' --image=myapp:latest                   | Маніфест для створення CronJob.                              | [app-cronjob.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-cronjob.yaml) |
| app-job.yaml           | create job myjob --image=myapp:latest                       | Маніфест для створення одноразового завдання (Job).          | [app-job.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-job.yaml)         |
| app-multicontainer.yaml| create deploy myapp --image=myapp:latest --multi-container       | Маніфест для створення Pod з декількома контейнерами.        | [app-multicontainer.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-multicontainer.yaml) |
| app-resources.yaml     | create deploy myapp --image=myapp:latest --resources | Маніфест з налаштуванням ресурсів (requests and limits).     | [app-resources.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-resources.yaml) |
| app-secret-env.yaml    | create deploy myapp --image=myapp:latest --secret-env | Маніфест з налаштуванням секретних змінних середовища.       | [app-secret-env.yaml](https://github.com/roman-98/kube-ai/blob/main/yaml/app-secret-env.yaml) |

