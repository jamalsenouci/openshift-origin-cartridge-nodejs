# NodeJS Downloadable Cart
This cartridge is meant to represent a downloadable fork of the upstream [OpenShift Origin Nodejs Cartridge](https://github.com/openshift/origin-server/tree/master/cartridges/openshift-origin-cartridge-nodejs), which is documented in the [Cartridge Guide](http://openshift.github.io/documentation/oo_cartridge_guide.html#nodejs).

Launch it with:

```bash
rhc app create mynodeapp https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml
```

Or, for a more advanced example:

```bash
rhc app create nodejs https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml postgresql-9.2 --from-code=http://github.com/ryanj/restify-postGIS.git
```

You can even [launch it on the web](https://openshift.redhat.com/app/console/application_types/custom?cartridges[]=https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml): https://openshift.redhat.com/app/console/application_types/custom?name=parks&initial_git_url=https%3A%2F%2Fgithub.com/ryanj/restify-postGIS.git&cartridges[]=https://raw.githubusercontent.com/ryanj/openshift-origin-cartridge-nodejs/master/metadata/manifest.yml&cartridges[]=postgresql-9.2
