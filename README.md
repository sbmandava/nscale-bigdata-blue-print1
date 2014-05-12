# nScale BigData BluePrint #1 
Reference blueprint, which is highly optimized to build a multi-tier server farm on a local linux server
Components include a) Network Loadbalancer b) Webserver c) Hadoop (HDFS/Hive/Hbase d) Search Analytics (Elastic Search/Kibana)  

# Environment
Linux Server (Debian Wheezy) - Can be loaded inside VirtualBox.
Docker 0.11+

# Folder Structure
sbin/ - master initialization/cleanup scripts
bin/ - run time scripts.
etc/ - configuration store
build/ - image build folder
tmp/ - temporary files

# Startup Instructions
1) set path for folder in etc/env.conf
2) for each folder in build/ 
   - follow instructions in the folder/readme-build to build the images.
3) ensure that "docker images" shows the build images
4) Initialize the network setup
    edit etc/net-setup.conf
    sbin/init-network
