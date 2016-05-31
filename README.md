## PyCon Taiwan 2016

## Strategies for concurrency and parallelism in Python

### Demo files
### python 2.7

#### Synchronous
```python
python synchronous.py
```

#### Multiple thread
```python
python multipleThreads.py
```

#### Multiple process
```python
python multipleProcesses.py
```

#### RQ worker

- Install vagrant
- Install chef-dk for berkshelf https://downloads.chef.io/chef-dk/mac/#/
- Run
```
vagrant plugin install vagrant-berkshelf
vagrant plugin install vagrant-omnibus
berks install
vagrant up
vagrant provision
vagrant ssh
cd vagrant
. set_env.sh
python rqworker.py
```
- Run in another terminal session at folder root
```
python rqworker_client.py
```
