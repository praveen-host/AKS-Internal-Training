<b>Volumes</b></br>
Kubernetes volumes are a component of a pod and are thus defined in the pod’s specification—much like containers. They aren’t a standalone Kubernetes object and cannot be created or deleted on their own. A volume is available to all containers in the
pod, but it must be mounted in each container that needs to access it. In each container, you can mount the volume in any location of its filesystem.

<b>Volume Types</b></br>
 emptyDir—A simple empty directory used for storing transient data.</br>
 hostPath—Used for mounting directories from the worker node’s filesystem into the pod.</br>
 gitRepo—A volume initialized by checking out the contents of a Git repository.</br>
 nfs—An NFS share mounted into the pod.</br>
 gcePersistentDisk (Google Compute Engine Persistent Disk), awsElasticBlockStore (Amazon Web Services Elastic Block Store Volume), azureDisk (Microsoft Azure Disk Volume)—Used for mounting cloud provider-specific storage.</br>
 cinder, cephfs, iscsi, flocker, glusterfs, quobyte, rbd, flexVolume, vsphereVolume, photonPersistentDisk, scaleIO—Used for mounting other types of network storage.</br>
 configMap, secret, downwardAPI—Special types of volumes used to expose certain Kubernetes resources and cluster information to the pod.</br>
 persistentVolumeClaim—A way to use a pre- or dynamically provisioned persistent storage.</br>
