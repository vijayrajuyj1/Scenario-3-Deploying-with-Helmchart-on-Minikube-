# Scenario-3-Deploying-with-Helm-on-Minikube

# 📌 Task

**Create a Helm chart to deploy the container from Scenario 2 on Minikube.**

**✅ Requirements**

The pod should not auto-execute but must allow bash access for manual execution.

# 🛠 Prerequisites

**Before running this project, make sure you have the following installed:**

1.Minikube

2.Helm

3.Kubectl

4.Docker

**📥 Clone the Repository**

```bash
git clone https://github.com/vijayrajuyj1/Scenario-3-Deploying-with-Helm-on-Minikube.git
```

**🚀 Setup and Start Minikube**

```bash
$ minkube start
```

**🎩 Deploy with Helm**

```
$ helm create demochart
```
**Note: Perform all the changes and update the all files after that use below command**

```bash
$ helm install task3 demochart
```

**🔍 Verify Deployment**

```bash
$ kubectl get pods
```

**⚡️ Access the Pod for Manual Execution**

```bash
$ kubeclt exec -it <pod name> -- /bin/sh
```

**Inside the pod  manually run your Star Wars API Scanner script**

```bash
python3 starships_pilots.py "A New Hope"
```

**Expected Output (JSON Format)**

```json
{
    "film": "A new Hope",
    "starships": [
        {
            "starship": "CR90 corvette",
            "pilots": []
        },
        {
            "starship": "Star Destroyer",
            "pilots": []
        },
        {
            "starship": "Sentinel-class landing craft",
            "pilots": []
        },
        {
            "starship": "Death Star",
            "pilots": []
        },
        {
            "starship": "Millennium Falcon",
            "pilots": [
                "Chewbacca",
                "Han Solo",
                "Lando Calrissian",
                "Nien Nunb"
            ]
        },
        {
            "starship": "Y-wing",
            "pilots": []
        },
        {
            "starship": "X-wing",
            "pilots": [
                "Luke Skywalker",
                "Biggs Darklighter",
                "Wedge Antilles",
                "Jek Tono Porkins"
            ]
        },
        {
            "starship": "TIE Advanced x1",
            "pilots": [
                "Darth Vader"
            ]
        }
    ]
}
```


### 📩 Contact

**Vijayaraju Devops and Cloud Engineer**  
📧 Email: [vijayaraju7360@gmail.com](mailto:vijayaraju7360@gmail.com)



