# kube8

#successfully built my kubernetes cluter using kubeadm

#sudo apt install docker.io -y

#sudo systemctl start docker
#sudo systemctl enable docker

#kubeadm setup
#sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg
#echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list

#the public key is not availabe: NO_PUBKEY
#sudo apt-get install -y apt-transport-https ca-certificates curl
#curl -L https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key --keyring /usr/share/keyrings/cloud.google.gpg add
#sudo touch /etc/apt/sources.list.d/kubernetes.list
#sudo chmod 666 /etc/apt/sources.list.d/kubernetes.list
#sudo echo deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://apt.kubernetes.io/ kubernetes-xenial main | tee /etc/apt/sources.list.d/kubernetes.list
#sudo apt-get update

#sudo apt install kubeadm=1.20.0-00 kubectl=1.20.0-00 kubelet=1.20.0-00 -y
#or
#sudo apt-get install -y kubelet kubeadm kubectl
#sudo su
#kubeadm init  'if this commont is not working then try this"
#sudo systemctl stop kubelet.service  #kubeadm reset  #kubeadm init --v=5
#use export kubeconfig
#kubectl apply -f https://github.com/weaveworks/weave/releases/download/v2.8.1/weave-daemonset-k8s.yaml
#kubeadm token create --print-join-command
#master nodes 
#sudo su 
#kubeadm reset pre-flight checks
#kubectl get nodes
#kubectl run nginx --image=nginx --restart=Never
#kubectl get pod
#kubectl delete -f file-name

error kubectl get nodes :-The connection to the server localhost:8080 was refused - did you specify the right host or port?
# curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl
# sudo cp /etc/kubernetes/admin.conf /home/vagrant/config this comma path in different in your pc you can also use this sudo cp -i /etc/kubernetes/admin.conf $HOME/.kube/config then cd .kube and check
#mkdir .kube
# ll
# cat admin.conf
# sudo kubectl get nodes
# sudo cp admin.conf config
# mv config .kube/
# sudo chown $(id -u):$(id -g) $HOME/.kube/config

#kubectl get namespaces
#kubectl get pods -ns=kube-system
#kubectl get ns
#kubectl get pods -ns=default
#kubectl create namespaces group-name
#kubectl apply -f file-name 
#kubectl get pods -n=name-space-ns
#kubectl delete -f podname.yml
#kubectl get pods -o wide -n name-space-ns
#kubectl get service
#kubectl get service -n name-space-ns
#kubectl get pods -n name-space-ns
#kubectl describe deployment.apps/dfile-name-deployment -n name-space-ns
#kubectl create namespace mysql-db
#kubectl get secret -n mysql-db

#create key
#the public key is not available: NO_PUBKEY 
#sudo apt-get install launchpad-getkeys 
#sudo launchpad-getkeys 
#sudo apt update -y
#sudo add-apt-repository --remove ppa:whatever/ppa
#sudo apt update -y
#sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys
#sudo apt-get update -y
#echo 'password' | base64
#echo 'encPass' | base64 --decode

Kubernetes.io/docs
