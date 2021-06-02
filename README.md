<img src="components/logo-small.png"><br><img src="https://img.shields.io/github/issues/lnxpy/bluelight?style=square" alt="Version" style="max-width:100%;"> <img src="https://img.shields.io/github/stars/lnxpy/bluelight?style=square" alt="Version" style="max-width:100%;"> <img src="https://img.shields.io/github/license/lnxpy/bluelight?color=purple&style=square" alt="Version" style="max-width:100%;">

BlueLight concept explains the base infrastructure explanation in the IoT with [Socket](https://docs.python.org/3/library/socket.html) and [Django](https://www.djangoproject.com/) webserver which proves that you can control your house lighting system using a simple small private network with a Django service and a device to control the operations. (PC, Laptop, Smartphone, etc)

All you need is a [RaspberryPi](https://www.raspberrypi.org/) to run up the Django webserver and a private network. In most cases, a wireless network is recommandad.

### Infrastructure
All the controller devices should be in the same network as the webserver. There is an API service running on the server that has multiple included socket tasks through the [Celery](https://docs.celeryproject.org/en/stable/getting-started/introduction.html) functions and connected to a [RabbitMQ](https://www.rabbitmq.com/) to keep the queues. In this case, Celery allows you to make the schedules. Something much more advanced. BlueLight uses the following structure.
