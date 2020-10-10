# iot-rpi-k8s-

IoT application 
Iot edge node is RasberryPi where run mqtt image
On k8s cluster run mqtt broker and nodered to control rasberrypi.

Test mqtt
k8s - 
kubectl exec (pod-id) -i -t -- mosquitto_sub -h localhost -v -t "testing/"

from rpi
 docker exec (container-id) mosquitto_pub -h 192.168.14.11 -p 30884 -t "testing/" -m "Testing bridged brokers!"
