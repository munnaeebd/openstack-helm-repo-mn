# openstack-helm-repo-mn
openstack-helm-repo-mn

~~~
mkdir {git,openstack-helm}
cd openstack-helm
git clone https://github.com/openstack/openstack-helm.git
git clone https://github.com/openstack/openstack-helm-infra.git


helm serve & 
cd  openstack-helm-infra
make helm-toolkit
make ingress
make {openvswitch,mariadb,libvirt,rabbitmq,memcached}
cd ../openstack-helm
make {keystone,horizon,glance,cinder,nova,placement,neutron,heat} 

 cd ~/git/
 git clone https://github.com/munnaeebd/openstack-helm-repo-mn.git

cp  ~/openstack-helm/openstack-helm/*.tgz ~/git/openstack-helm-repo-mn/
cp  ~/openstack-helm/openstack-helm-infra/*.tgz ~/git/openstack-helm-repo-mn/


~~~


