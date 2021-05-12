<img src="components/logo-small.png"><br><img src="https://img.shields.io/github/issues/lnxpy/bluelight?style=square" alt="Version" style="max-width:100%;"> <img src="https://img.shields.io/github/stars/lnxpy/bluelight?style=square" alt="Version" style="max-width:100%;"> <img src="https://img.shields.io/github/license/lnxpy/bluelight?color=purple&style=square" alt="Version" style="max-width:100%;">

BlueLight conecept explains the base infrastucture explanation in the IoT with [Socket]() and [Django]() webserver which proves that you can control your house lighing system using a simpe small private network with a Django service and a device to control the operations. (PC, Laptop, Smartphone, etc)

All you need is a [RaspberryPi]() to run up the Django webserver and a private network. In most cases, a wireless network is recommandad.

### Infrastructure
All the controller devices should be in the same network as the webserver. There is an API service running on the server that has multiple included socket tasks through the [Celery]() functions and connected to a [RabbitMQ]() to keep the queues. In this case, Celery allows you to make the schedules. Something much more advance.
