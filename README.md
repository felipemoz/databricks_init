# blobfuse mount init script
Inspired by https://github.com/Azure/azure-storage-fuse, this notebook creates an init script that mounts an Azure Blob Storage container with blobfuse on a cluster:

1. Import this notebook to your workspace.
2. Edit the variables above
3. Change the block of cell 8 using your own script
6. Run this notebook (clicking **Run All** above). It will generate a script called `blobfuse-mount.sh` in the location you provided.

To create a cluster with the mount:
1. Configure a cluster with the `blobfuse-mount.sh` cluster-scoped init script [using the UI](https://docs.azuredatabricks.net/user-guide/clusters/init-scripts.html#cluster-scoped-init-scripts), [Databricks CLI](https://docs.azuredatabricks.net/user-guide/dev-tools/databricks-cli.html#databricks-cli), or by [invoking the Clusters API](https://docs.azuredatabricks.net/api/latest/clusters.html#cluster-api). 
2. Start the cluster.
