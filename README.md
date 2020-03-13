## Welcome to Openstorage-CSI

This organization contains all of the open source forks of Kubernetes CSI components by Portworx. All forked releases are built off of existing Kubernetes-CSI releases. For example, our External Provisioner v1.4.0-1 release contains all changes in v1.4.0, with a few extra changes (-1). 

Currently, have the following fork releases with minor changes.
1. [External Provisioner v1.4.0-1](https://github.com/openstorage-csi/external-provisioner/releases/tag/v1.4.0-1)
  * add PVC Metadata to req.Parameters for openstorage
  * Separate PVC labels and annotations

2. [External Snapshotter v1.2.2-1](https://github.com/openstorage-csi/external-snapshotter/releases/tag/v1.2.2-1)
  * perform an os.Exit when the CSI gRPC connection is lost
  * Add support for configmaps leaderelection for k8s 1.13

3. [External Attacher v1.2.1-1](https://github.com/openstorage-csi/external-attacher/releases/tag/v1.2.1-1)
  * perform an os.Exit when the CSI gRPC connection is lost. This change is only in v2.0.0+ versions of the official sidecar, which has a minimum k8s version of 1.14.
