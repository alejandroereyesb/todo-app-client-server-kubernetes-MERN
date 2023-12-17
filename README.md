# React, Node Js, and MongoDB microservices-based application deployment on Kubernetes

This complete article can be check at [medium.com/@aamirpinger](https://medium.com/@aamirpinger/react-express-node-js-and-mongodb-mern-stack-microservices-based-application-deployment-on-ec4607cec74d)

This is a simple ToDo application build using MERN Stack. It consist of:
1. The Front-end application is build using React.
2. The backend is build using Node Js, Express, and mongoose.
3. The Database Layer will be using the NoSQL database i.e. MongoDB.

As a brief overview of this todo app, when the user will access the front-end application from the browser, a login screen with a signup option appears. User must first signup to register and then after having success on signup can login into the app by using registered email and the password.

After a successful login, user will then add a new Todo task and list already added todos. Users can also mark any specific ToDo as important by clicking on the star, mark them as completed, and delete any specific ToDo when needed. Users may also use the ToDo search option and sort the paginated list on serial no, title, or description.

# General commands

Run Minikube
> minikube start

Shut down Minikube
> minikube stop

Obtain IP Minikube. You should get something like `192.168.49.2`
> minikube ip

Open minikube dashboard
> minikube dashboard         

Check services
> kubectl get service

Check pods
> kubectl get pod

Check deployments
> kubectl get deploy

Check general info
> kubectl get deploy

Open website portal. Example: `http://192.168.49.2:32608/`
> minikube_ip:port_web_service

To scale up or down front-end application
> kubectl scale deploy todo-client-app-deploy --replicas=<count>

To scale up or down backend application
> kubectl scale deploy todo-server-app-deploy --replicas=<count>