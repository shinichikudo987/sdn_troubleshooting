# Some useful commands for create the topology using physic SDN switch

## Topology
```
http://www.topology-zoo.org/maps/Packetexchange.jpg
```

## Assign the IP for SDN switch
```
dhclient -v eth0
```

## Restart service
```
service picos restart
```

## Delete bridge
```
ovs-vsctl del-br sw1
ovs-vsctl del-br sw2
ovs-vsctl del-br sw3
ovs-vsctl del-br sw4
ovs-vsctl del-br sw5
ovs-vsctl del-br sw6
ovs-vsctl del-br sw7
ovs-vsctl del-br sw8
ovs-vsctl del-br sw9
ovs-vsctl del-br sw10
ovs-vsctl del-br sw11
ovs-vsctl del-br sw12
```

## Create physical node in SDN switch
```
ovs-vsctl  add-br sw1 -- set bridge sw1 datapath_type=pica8 
ovs-vsctl  add-port sw1 ge-1/1/1 vlan_mode=access -- set Interface ge-1/1/1 type=pica8
ovs-vsctl  add-port sw1 ge-1/1/2 vlan_mode=access -- set Interface ge-1/1/2 type=pica8
ovs-vsctl  add-port sw1 ge-1/1/3 vlan_mode=access -- set Interface ge-1/1/3 type=pica8
ovs-vsctl  add-port sw1 ge-1/1/4 vlan_mode=access -- set Interface ge-1/1/4 type=pica8
ovs-vsctl  set-controller sw1 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw1 protocol=OpenFlow10


ovs-vsctl  add-br sw2 -- set bridge sw2 datapath_type=pica8 
ovs-vsctl  add-port sw2 ge-1/1/5 vlan_mode=access -- set Interface ge-1/1/5 type=pica8
ovs-vsctl  add-port sw2 ge-1/1/6 vlan_mode=access -- set Interface ge-1/1/6 type=pica8
ovs-vsctl  add-port sw2 ge-1/1/7 vlan_mode=access -- set Interface ge-1/1/7 type=pica8
ovs-vsctl  add-port sw2 ge-1/1/8 vlan_mode=access -- set Interface ge-1/1/8 type=pica8
ovs-vsctl  set-controller sw2 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw2 protocol=OpenFlow10


ovs-vsctl  add-br sw3 -- set bridge sw3 datapath_type=pica8 
ovs-vsctl  add-port sw3 ge-1/1/9 vlan_mode=access -- set Interface ge-1/1/9 type=pica8
ovs-vsctl  add-port sw3 ge-1/1/10 vlan_mode=access -- set Interface ge-1/1/10 type=pica8
ovs-vsctl  add-port sw3 ge-1/1/11 vlan_mode=access -- set Interface ge-1/1/11 type=pica8
ovs-vsctl  add-port sw3 ge-1/1/12 vlan_mode=access -- set Interface ge-1/1/12 type=pica8
ovs-vsctl  set-controller sw3 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw3 protocol=OpenFlow10


ovs-vsctl  add-br sw4 -- set bridge sw4 datapath_type=pica8 
ovs-vsctl  add-port sw4 ge-1/1/13 vlan_mode=access -- set Interface ge-1/1/13 type=pica8
ovs-vsctl  add-port sw4 ge-1/1/14 vlan_mode=access -- set Interface ge-1/1/14 type=pica8
ovs-vsctl  add-port sw4 ge-1/1/15 vlan_mode=access -- set Interface ge-1/1/15 type=pica8
ovs-vsctl  add-port sw4 ge-1/1/16 vlan_mode=access -- set Interface ge-1/1/16 type=pica8
ovs-vsctl  set-controller sw4 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw4 protocol=OpenFlow10


ovs-vsctl  add-br sw5 -- set bridge sw5 datapath_type=pica8 
ovs-vsctl  add-port sw5 ge-1/1/17 vlan_mode=access -- set Interface ge-1/1/17 type=pica8
ovs-vsctl  add-port sw5 ge-1/1/18 vlan_mode=access -- set Interface ge-1/1/18 type=pica8
ovs-vsctl  add-port sw5 ge-1/1/19 vlan_mode=access -- set Interface ge-1/1/19 type=pica8
ovs-vsctl  add-port sw5 ge-1/1/20 vlan_mode=access -- set Interface ge-1/1/20 type=pica8
ovs-vsctl  set-controller sw5 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw5 protocol=OpenFlow10


ovs-vsctl  add-br sw6 -- set bridge sw6 datapath_type=pica8 
ovs-vsctl  add-port sw6 ge-1/1/21 vlan_mode=access -- set Interface ge-1/1/21 type=pica8
ovs-vsctl  add-port sw6 ge-1/1/22 vlan_mode=access -- set Interface ge-1/1/22 type=pica8
ovs-vsctl  add-port sw6 ge-1/1/23 vlan_mode=access -- set Interface ge-1/1/23 type=pica8
ovs-vsctl  add-port sw6 ge-1/1/24 vlan_mode=access -- set Interface ge-1/1/24 type=pica8
ovs-vsctl  set-controller sw6 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw6 protocol=OpenFlow10


ovs-vsctl  add-br sw7 -- set bridge sw7 datapath_type=pica8 
ovs-vsctl  add-port sw7 ge-1/1/25 vlan_mode=access -- set Interface ge-1/1/25 type=pica8
ovs-vsctl  add-port sw7 ge-1/1/26 vlan_mode=access -- set Interface ge-1/1/26 type=pica8
ovs-vsctl  add-port sw7 ge-1/1/27 vlan_mode=access -- set Interface ge-1/1/27 type=pica8
ovs-vsctl  add-port sw7 ge-1/1/28 vlan_mode=access -- set Interface ge-1/1/28 type=pica8
ovs-vsctl  set-controller sw7 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw7 protocol=OpenFlow10

ovs-vsctl  add-br sw8 -- set bridge sw8 datapath_type=pica8 
ovs-vsctl  add-port sw8 ge-1/1/29 vlan_mode=access -- set Interface ge-1/1/29 type=pica8
ovs-vsctl  add-port sw8 ge-1/1/30 vlan_mode=access -- set Interface ge-1/1/30 type=pica8
ovs-vsctl  add-port sw8 ge-1/1/31 vlan_mode=access -- set Interface ge-1/1/31 type=pica8
ovs-vsctl  add-port sw8 ge-1/1/32 vlan_mode=access -- set Interface ge-1/1/32 type=pica8
ovs-vsctl  set-controller sw8 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw8 protocol=OpenFlow10

ovs-vsctl  add-br sw9 -- set bridge sw9 datapath_type=pica8 
ovs-vsctl  add-port sw9 ge-1/1/33 vlan_mode=access -- set Interface ge-1/1/33 type=pica8
ovs-vsctl  add-port sw9 ge-1/1/34 vlan_mode=access -- set Interface ge-1/1/34 type=pica8
ovs-vsctl  add-port sw9 ge-1/1/35 vlan_mode=access -- set Interface ge-1/1/35 type=pica8
ovs-vsctl  add-port sw9 ge-1/1/36 vlan_mode=access -- set Interface ge-1/1/36 type=pica8
ovs-vsctl  set-controller sw9 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw9 protocol=OpenFlow10

ovs-vsctl  add-br sw10 -- set bridge sw10 datapath_type=pica8 
ovs-vsctl  add-port sw10 ge-1/1/37 vlan_mode=access -- set Interface ge-1/1/37 type=pica8
ovs-vsctl  add-port sw10 ge-1/1/38 vlan_mode=access -- set Interface ge-1/1/38 type=pica8
ovs-vsctl  add-port sw10 ge-1/1/39 vlan_mode=access -- set Interface ge-1/1/39 type=pica8
ovs-vsctl  add-port sw10 ge-1/1/40 vlan_mode=access -- set Interface ge-1/1/40 type=pica8
ovs-vsctl  set-controller sw10 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw10 protocol=OpenFlow10

ovs-vsctl  add-br sw11 -- set bridge sw11 datapath_type=pica8 
ovs-vsctl  add-port sw11 ge-1/1/41 vlan_mode=access -- set Interface ge-1/1/41 type=pica8
ovs-vsctl  add-port sw11 ge-1/1/42 vlan_mode=access -- set Interface ge-1/1/42 type=pica8
ovs-vsctl  add-port sw11 ge-1/1/43 vlan_mode=access -- set Interface ge-1/1/43 type=pica8
ovs-vsctl  add-port sw11 ge-1/1/44 vlan_mode=access -- set Interface ge-1/1/44 type=pica8
ovs-vsctl  set-controller sw11 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw11 protocol=OpenFlow10

ovs-vsctl  add-br sw12 -- set bridge sw12 datapath_type=pica8 
ovs-vsctl  add-port sw12 ge-1/1/45 vlan_mode=access -- set Interface ge-1/1/45 type=pica8
ovs-vsctl  add-port sw12 ge-1/1/46 vlan_mode=access -- set Interface ge-1/1/46 type=pica8
ovs-vsctl  add-port sw12 ge-1/1/47 vlan_mode=access -- set Interface ge-1/1/47 type=pica8
ovs-vsctl  add-port sw12 ge-1/1/48 vlan_mode=access -- set Interface ge-1/1/48 type=pica8
ovs-vsctl  set-controller sw12 tcp:10.12.20.158:6633
ovs-vsctl  set bridge sw12 protocol=OpenFlow10
```

## List all controllers and status
```
ovs-vsctl list controller
```


