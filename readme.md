# Deploy
kubectl apply -f config.yaml -f postgres.yaml -f initdb.yaml -f deployment.yaml -f service.yaml -f ingress.yaml

## Паттерн идемпотентности
Версионирование на основе id последнего заказа (lastOrderId).<br />
Получение lastOrderId происходит путем запроса:<br />
GET /otusapp/order
