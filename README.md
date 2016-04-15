# Openvswitch

## install

```bash
apt-get install -y  openvswitch-switch
```

## ovs-vsctl

This tool is used for configuring the ovs-vswitchd configuration database (known as ovs-db)

### Create a virtual switch

```bash
ovs-vsctl add-br mybridge
```


Prints a list of configured bridges
```bash
ovs-vsctl list-br
```


display virtual switch database configuration

```bash
ovs-vsctl show
```

### add port

```bash
ovs-vsctl add-port mybridge eth0
```

### delete a bridge

```bash
ovs-vsctl del-br mybridge
```



## ovs-ofctl

A command line tool for monitoring and administering OpenFlow switches