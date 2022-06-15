<!-- toc -->

# Frequently Asked Questions

The following page hosts some frequently asked questions as noticed in our [issues](https://github.com/CybersecurityLuxembourg/openxeco-core/issues).

***
## General questions
### Where can I get support?

If you have feature requests or you found a bug you can open a ticket on [openXeco's GitHub repository issue](https://github.com/CybersecurityLuxembourg/openxeco-core/issues) tracker.

### What are the hardware requirements?

From a hardware perspective, openXeco's requirements are in the mid-range, a web server with 4+ cores and 16-24 GB of memory should be plenty, though more is always better of course. A lot of it depends on the data set and the number of users you are dealing with. 

We recommend a standard LAM stack on top of Ubuntu >20.04 LTS. For details on the exact dependencies please refer to the [installation guide](https://doc.openxeco.org/).


### How to monitor openXeco?

***
## Specific questions
### Can I configure openXeco to send encrypted notification mails


### How to change config of an already running Docker container?

In case you need to manually modify environment variables for example. The below can be done:

```
# Changin config for oxe-api container
D_ID=$(docker ps --no-trunc | grep oxe-api |cut -f1 -d\ )
docker stop ${D_ID}
sudo vi /var/lib/docker/containers/${D_ID}/config.v2.json
# ...
docker start ${D_ID}
```

[source](https://stackoverflow.com/questions/48059540/how-to-change-docker-config-of-an-already-running-container)
