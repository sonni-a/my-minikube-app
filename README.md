# Проектирование информационных систем
## Лабораторная работа №7. k8s 
Цель: ознакомить с k8s, развернуть сервис с использованием minicube

Задачи:
развернуть minicube 
создать docker образ вашего приложения;
создать deployment;
установить кол-во подов на 3
добавьте Metrics Server (kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml).
настройте Horizontal Pod Autoscaler (HPA), чтобы масштабировать поды при увеличении нагрузки (kubectl autoscale deployment my-app --cpu-percent=50 --min=2 --max=5).
 настройте Prometheus и Grafana через (helm install prometheus prometheus-community/kube-prometheus-stack). Настройте дашборды в Grafana для мониторинга нагрузки (хотя бы один)

1. Разворачиваем minikube на Linux Mint с драйвером docker
   ![](https://github.com/sonni-a/my-minikube-app/blob/main/img1.png?raw=true)
2. Создаем docker образ приложения
