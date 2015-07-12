## SimpleAnnotationServer with vagrant and ansible

Builds a ubuntu virtual machine and clones and runs [SimpleAnnotationServer](https://github.com/glenrobson/SimpleAnnotationServer).

Prerequisites
-------------

Have vagrant and ansible installed.

How to run
----------

Clone the repository

`git clone https://github.com/404mike/SimpleAnnotationServer.git`

cd into repository

`cd SimpleAnnotationServer`

Start vagrant

`vagrant up`

Once vagrant has finished building the vm, ssh into your new vm
`vagrant ssh`

cd into the SimpleAnnotationServer directory
`cd /vagrant/app/SimpleAnnotationServer/`

run the start command
`mvn jetty:run`

You should now be able to view the application in your browser [192.168.50.50:8888](http://192.168.50.50:8888)