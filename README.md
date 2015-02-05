# NodeJS Downloadable Cart
This cartridge is meant to represent a downloadable fork of the upstream [OpenShift Origin Nodejs Cartridge](https://github.com/openshift/origin-server/tree/master/cartridges/openshift-origin-cartridge-nodejs), which is documented in the [Cartridge Guide](http://openshift.github.io/documentation/oo_cartridge_guide.html#nodejs).

Provide your own git repo url to [create embeddable launch buttons that use this cart](http://launch-shifter.rhcloud.com/?cartridges[]=https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.ymlhttps://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.ymlhttps://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.ymlhttps://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml&initial_git_url=https://github.com/ryanj/restify-base.git&name=noderestify): 

[![LAUNCH ON OpenShift](http://launch-shifter.rhcloud.com/launch/LAUNCH ON.svg)](https://openshift.redhat.com/app/console/application_type/custom?cartridges[]=https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml&initial_git_url=https://github.com/ryanj/restify-base.git&name=noderestify)

To run this container environment from the command line with it's default 'hello world' content:

```bash
rhc app create mynodeapp https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml
```

To incorporate an initial git repo, use the `--from-code` flag:

```bash
rhc app create noderestify https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml --from-code=http://github.com/ryanj/restify-base.git
```

Multi-container example w/ postgreSQL: https://openshift.redhat.com/app/console/application_types/custom?name=parks&initial_git_url=https%3A%2F%2Fgithub.com/ryanj/restify-postGIS.git&cartridges[]=https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml&cartridges[]=postgresql-9.2

```bash
rhc app create pgparks https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml postgresql-9.2 --from-code=http://github.com/ryanj/restify-postGIS.git
```
