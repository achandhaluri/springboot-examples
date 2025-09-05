docker build -t your-dockerhub-username/spring-boot-student-event:latest .
docker run --rm -p 8080:8080 your-dockerhub-username/spring-boot-student-event:latest 

kubectl apply -f k8s/manifest.yaml
kubectl -n student-event get pods,svc
kubectl -n student-event port-forward svc/student-event-svc 8080:80

kubectl apply -f k8s/manifest.yaml
kubectl -n student-event get pods,svc
kubectl -n student-event port-forward svc/student-event-svc 8080:80

PlantUML source: docs/uml/student-event.puml

Mermaid version (renders on GitHub): docs/uml/README.md
