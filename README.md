
A small extenstion to retrieve upstream source informations for all
containers in your cluster.

## Prepare

1. Create a token here: https://access.redhat.com/terms-based-registry/
2. Then do podman login: `podman login -u='$TOKEN_NAME' -p=$TOKEN_VALUE`

## Usage

After logging into the OpenShift cluster you can run:

    $ oc-get-upstream-sources all
    …

In order to fetch all the upstream source informations for all container images
currently being used on the cluster - if the container is providing this information.
