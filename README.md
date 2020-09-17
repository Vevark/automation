# automation
Self-modified ACC course material
The original link is https://github.com/SNICScienceCloud/technical-training/tree/master/automation

## Task 4
run the command
```bash
apt-get install python3-heatclient
```
before
```bash
openstack stack create stack_with_init_script -f ‘yaml’ -t ssc-test-stack.yml 
```

## Task 5
After failed to RUN apt-get update
```bash
sudo bash
vi /etc/docker/daemon.json
{
"mtu": 1400
}

service docker restart
docker build --no-cache -t cowsay:latest .
docker run -d -p 5000:5000  cowsay
```
