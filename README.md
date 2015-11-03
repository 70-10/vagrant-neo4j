Vagrant-Neo4j
===

Neo4j Playbook and Vagrant Setup

## Usage

### Vagrant

```
$ cd localvm
$ vagrant up
```

### Job for upstart

#### list

```
$ initctl list | grep neo4j
```

#### start

```
$ initctl start neo4j
```

#### stop

```
$ initctl stop neo4j
```

### Access Neo4j

http://neo4j.local:7474/ or http://172.17.5.100:7474/
