bitcoinbeacon
=============
A project to create a public randomness beacon using the bitcoin blockchain and block hashes as the basis for randomness.

---

## Execution
```
dev_appserver.py --clear_datastore=yes app.yaml
```
Reference https://cloud.google.com/appengine/docs/standard/python/tools/using-local-server

## Setup
### Install required modules for python
```
sudo pip install jinja2
sudo pip install ndb
sudo pip install webob
sudo pip install webapp2
...
```

### Install google sdk 

- https://cloud.google.com/appengine/docs/standard/python/download

Below instruction is for DEBIAN/UBUNTU
```
export CLOUD_SDK_REPO="cloud-sdk-$(lsb_release -c -s)"
echo "deb https://packages.cloud.google.com/apt $CLOUD_SDK_REPO main" | sudo tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
sudo apt-get update && sudo apt-get install google-cloud-sdk
sudo apt-get install google-cloud-sdk-app-engine-python
```

