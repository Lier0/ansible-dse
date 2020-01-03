# ansible-dse-node

Create dse-node cluster, with graph enabled.
Designed to be on a crypted network (ie no crypting services enabled about dse).

## Vars
```
dse_cluster_name: dse-node-cluster                 
dse:                                 
  username: ''
  password: ''              
  stomp: "{{ hostvars[groups['opscenter'][0]]['ansible_eth0']['ipv4']['address']
dse_port:                                                                       
  cql: 9042                                                                     
  grem: 8182   
```
