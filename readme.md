# Deploy
kubectl apply -f config.yaml -f postgres.yaml -f initdb.yaml -f deployment.yaml -f service.yaml -f ingress.yaml

## Паттерн идемпотентности
Версионирование на основе id последнего заказа (lastOrderId).
Получение lastOrderId происходит путем запроса:
GET /otusapp/order
