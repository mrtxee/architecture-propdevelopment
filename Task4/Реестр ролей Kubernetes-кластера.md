# Реестр ролей Kubernetes-кластера PropDevelopment

## Роли кластера и их назначение

| Роль           | Права роли                                                                                              | Группы пользователей                   |
|----------------|---------------------------------------------------------------------------------------------------------|----------------------------------------|
| dev-admin      | Все действия над ресурами pods, services, configmaps, deployments, replicasets в пределах namespace dev | Тимлид команды, некоторые разработчики |
| cluster-admin  | Все действия над ресурами pods, services, configmaps, deployments, replicasets в пределах кластера      | Девопсы                                |
| cluster-viewer | Действия get, list, watch над ресурами pods, services, configmaps в пределах кластера                   | Разработчики, тестировщики, аналитики  |
| auditor-reader | Действия get, list, watch над ресурами pods, events, secrets в пределах кластера                        | СИБ                                    |
