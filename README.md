# DevOps-for-IBM-Cloud-Private


## Managing workloads
- Creating DaemonSets 
- Managing deployments 
- Managing Helm releases 
- Managing jobs 
- Creating StatefulSets 
- Managing ReplicaSets 

## [Managing charts and apps](https://www.ibm.com/support/knowledgecenter/SSBS6K_2.1.0.3/app_center/app_center.html)
The Catalog displays Helm charts, which contain application packages that can run as Kubernetes services. By using the Catalog, you can browse and install packages in your IBM® Cloud Private cluster (IPC) from Helm charts.

The packages are stored in repositories and IBM Cloud Private contains one repository connection by default. However can connect to other repositories to Catalog which will allow their Charts to be accessed from the Catalog as well

As Application developers develop applications these applications can also be published to the Catalog so that other users can easily install and access these applications.

> To deploy a Helm chart, it requires elevated privileges, Cluster Administrator, 
> from the IBM® Cloud Private Catalog to assigned namespaces that contain defined pod security policies.

> See [Accessing your IBM® Cloud Private cluster by using the kubectl CLI](https://www.ibm.com/support/knowledgecenter/SSBS6K_2.1.0.3/manage_cluster/cfc_cli.html)
> You also may need to setup a [Service Account](https://www.ibm.com/developerworks/community/blogs/fe25b4ef-ea6a-4d86-a629-6f87ccf4649e/entry/Configuring_the_Kubernetes_CLI_by_using_service_account_tokens1?lang=en)

Each Helm chart can be filtered based on the following classifications:
- Repository name

- Architecture
  - Linux® 64-bit
  - Linux® on Power® (ppc64le)
  - IBM® Z

- Release type
  - Beta - Early release charts that are officially announced.
  - Tech Preview - Charts that are not yet announced but available for early review.
  - Limited use - Charts that can be used for development trials and evaluations(no charge charts)
  - Commercial use - Charts that can be used for production (paid charts)

## Managing images

## Managing your platform
