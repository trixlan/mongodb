MongoDB Container for OpenShift 3
=================================

Version of a popular MongoDB Docker image (docker pull spec: mongo)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The mongo docker image (at least version 3.4.9) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (mongodb-imagestream.yml) which will
import the mongo image(s) into the internal registry of an OpenShift
cluster.
