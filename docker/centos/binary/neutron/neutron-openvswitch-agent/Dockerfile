FROM %%KOLLA_NAMESPACE%%/%%KOLLA_PREFIX%%neutron-base
MAINTAINER Kolla Project (https://launchpad.net/kolla)

# Install required packages
RUN yum install -y openstack-neutron-openvswitch \
                   openvswitch \
    && yum clean all

COPY check.sh start.sh /

CMD ["/start.sh"]
