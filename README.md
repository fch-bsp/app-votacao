# Projeto Aplicação de Votação com __**Docker**__ e __**K8s**__: ☸🐳
 
 ## Candidatos a essa Eleição de 2022: __**Gato** 🐱__ e __**Cachorro**:🐶__ 
 
### O projeto usamos 5 Pods com estruturas Deployment-Service dentro de um namespace "vote" com as técnologias:

#### - Pod-Python
#### - Pod-Node.js
#### - Pod-Redis
#### - Pod-PostGreSQL
#### - Pod-.NET
 ---
 
 

![Untitled (3)](https://user-images.githubusercontent.com/102867453/164033071-79377945-2573-4adf-8c81-02afab534fd7.jpg)

---
##### Tela de Votação ☸ 😺🐶

![votacao](https://user-images.githubusercontent.com/102867453/164033886-2af1c30d-4ab7-4288-818e-fbfce72a745d.png)

---

##### Tela do Resultado da Votação ☸ 😺🐶

![result](https://user-images.githubusercontent.com/102867453/164033981-453d5ecf-be25-483b-8fb3-c21f554af542.png)

---

### Comandos usados para criação do Projeto: 👨🏻‍💻👨🏻‍💻


~~~yaml
1 kubectl create -f namespaces/vote.yaml  --save-config --record  
~~~
~~~yaml
2 kubectl create -f junção_app-dp/juncao_dp.yaml  --save-config --record
~~~
~~~yaml
3 kubectl create -f junção_app-svc/juncao_svc.yaml  --save-config --record 
~~~
~~~yaml
4 kubectl get all -n votacao 
~~~
~~~yaml
5 minikube service vote --url -n votacao   
~~~
~~~yaml
6 minikube service result --url -n votacao 
~~~
~~~yaml
7 kubectl get all -n votacao
~~~
~~~yaml
8 kubectl get po -n votacao
~~~
~~~yaml
9 kubectl get service -n votacao 
~~~
