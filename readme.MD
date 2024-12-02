# selectors

taints
------
* Newly creating pods won't create in taited node

kubectl taint nodes ip-192-168-19-108.ec2.internal hardware=gpu:NoSchedule

* Already existing pods will thrown out from the tainted node and create in another node

kubectl taint nodes ip-192-168-19-108.ec2.internal hardware=gpu:NoExecute

tolerance
----------

kubectl label nodes ip-192-168-19-108.ec2.internal hardware=gpu