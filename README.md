
# ROI Dashboard for vRealize Operations 8.1 and Cloud
---------

Use this [vRealize Operations](https://www.vmware.com/products/vrealize-operations.html) dashboard to view total cost of ownership, potential savings, and optimization costs.  View cost breakdown by cost drivers, capacity used, and datacenter as well as tracking for server depreciation.  More details on using this dashboard is available in the [ROI Dashboard for vRealize Operations](https://blogs.vmware.com/management/2020/05/roi-dashboard-for-vrealize-operations-8-1.html) blog post.

## Dashboard
![Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Dashboard.png)

## Installation
1. Install the [Reclaimable Resources Details Dashboard for vRealize Operations](https://vrealize.vmware.com/sample-exchange/vrealize-operations-sample-exchange/7039) dashboard according to the instructions on the dashboard page.
2. Install the [VM Rightsizing Details Dashboard for vRealize Operations](https://vrealize.vmware.com/sample-exchange/vrealize-operations-sample-exchange/6791) dashboard according to the instructions on the dashboard page.  Refer to the [Rightsizing VMs with vRealize Operations](https://blogs.vmware.com/management/2020/01/rightsizing-vms-with-vrealize-operations.html) blog post for a more detailed explanation of this dashboard.
3. Install the [Reclaimable Hosts Dashboard for vRealize Operations](https://vrealize.vmware.com/sample-exchange/vrealize-operations-sample-exchange/4981) dashboard according to the instructions on the dashboard page.
4. Import the super metrics at `Administration` / `Configuration` / `Super Metrics` / `Import Super Metric`  
![Import Super Metric](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Supermetric_Import.png)
5. Click `Browse...` then select the file named [supermetric.json](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/supermetric.json)
6. For each Super Metric listed in the [Super Metrics section](#Super-Metrics), click on the vertical kebab and select edit.  
![Policy Metrics](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Supermetric_Edit.png)
7. Enable the Super Metric for each Policy shown in the `Enable in a Policy` stage of the wizard.
![Policy Library](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Supermetric_Policy.png)
8. Repeat the previous 2 steps for the remaining Super Metrics listed in the [Super Metrics section](#Super-Metrics).
9. Import the view at `Dashboards` / `Views` / `Import...`  
![Import View](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/View_Import.png)
10. Click `Browse...` then select the file named [Views.zip](https://github.com/notoriousbdg/vrops-dashboard-roi/raw/master/Views.zip)
11. The included views are listed in the [Views section](#Views)
12. Import the dashboard at `Dashboards` / `Actions` / `Manage Dashboards` / `Import Dashboards`  
![Import Dashboard](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Dashboard_Import.png)
13. Click `Browse...` then select the file named [Dashboard.zip](https://github.com/notoriousbdg/vrops-dashboard-roi/raw/master/Dashboard.zip)
14. The dashboard should now be available in in the dashboard list  
![Dashboard List](https://raw.githubusercontent.com/notoriousbdg/vrops-dashboard-roi/master/images/Dashboard_List.png)
15. The included dashboards are listed in the [Dashboards section](#Dashboards)
16. Data should start showing after the first cost calculation completes.  Cost calculations run daily at 9 PM appliance time, which is UTC by default.
17. After a few days, the charts should start filling in as shown in the dashboard screenshot.

## Dashboards
| Dashboard Name | Dashboard Path |
|--|--|
| Return on Investment | Shared Dashboards (GBrandon)/Cost |

## Views
| View Name | Name on Dashboard | View Type |
|--|--|--|
| Cost Drivers Diagram | Reclaimable Hosts Detail | List |

## Super Metrics
| Super Metric Name | Object Type |
|--|--|
| Cost Drivers - Server Hardware (Owned) | vSphere World |
| Cost Drivers - Server Hardware (Owned) | Custom Datacenter |
| Cost Drivers - Server Hardware (Owned) | Datacenter |
| Cost Drivers - Server Hardware (Owned) | Cluster Compute Resource |
| Cost Drivers - Server Hardware (Leased) | vSphere World |
| Cost Drivers - Server Hardware (Leased) | Custom Datacenter |
| Cost Drivers - Server Hardware (Leased) | Datacenter |
| Cost Drivers - Server Hardware (Leased) | Cluster Compute Resource |
| Cost Drivers - Host OS License | vSphere World |
| Cost Drivers - Host OS License | Custom Datacenter |
| Cost Drivers - Host OS License | Datacenter |
| Cost Drivers - Host OS License | Cluster Compute Resource |
| Cost Drivers - Maintenance | vSphere World |
| Cost Drivers - Maintenance | Custom Datacenter |
| Cost Drivers - Maintenance | Datacenter |
| Cost Drivers - Maintenance | Cluster Compute Resource |
| Cost Drivers - Facilities | vSphere World |
| Cost Drivers - Facilities | Custom Datacenter |
| Cost Drivers - Facilities | Datacenter |
| Cost Drivers - Facilities | Cluster Compute Resource |
| Cost Drivers - Server Labor | vSphere World |
| Cost Drivers - Server Labor | Custom Datacenter |
| Cost Drivers - Server Labor | Datacenter |
| Cost Drivers - Server Labor | Cluster Compute Resource |
| Cost Drivers - Network | vSphere World |
| Cost Drivers - Network | Custom Datacenter |
| Cost Drivers - Network | Datacenter |
| Cost Drivers - Network | Cluster Compute Resource |
| Cost Drivers - Storage | vSphere World |
| Cost Drivers - Storage | Custom Datacenter |
| Cost Drivers - Storage | Datacenter |
| Cost Drivers - Storage | Cluster Compute Resource |
| Cost Drivers - VM Direct Costs | vSphere World |
| Cost Drivers - VM Direct Costs | Custom Datacenter |
| Cost Drivers - VM Direct Costs | Datacenter |
| Cost Drivers - VM Direct Costs | Cluster Compute Resource |
| Cost of Compute Capacity Remaining | vSphere World |
| Cost of Compute Capacity Used | vSphere World |
| Cost of Storage Capacity Remaining | vSphere World |
| Cost of Storage Capacity Used | vSphere World |
| Number of Fully Depreciated Servers | vSphere World |
| Number of Fully Depreciated Servers | Custom Datacenter |
| Number of Fully Depreciated Servers | Datacenter |
| Number of Fully Depreciated Servers | Cluster Compute Resource |
| Potential Savings and Optimization Opportunities | vSphere World |
| Total Cost of Ownership with Potential Savings and Optimizations | vSphere World |
| Total Potential Savings | vSphere World |
| Total Potential Savings | Custom Datacenter |
| Total Potential Savings | Datacenter |
| Total Potential Savings | Cluster Compute Resource |
| Total Server Purchase Cost | vSphere World |
| Total Server Purchase Cost | Custom Datacenter |
| Total Server Purchase Cost | Datacenter |
| Total Server Purchase Cost | Cluster Compute Resource |
| Total Server Accumulated Depreciation | vSphere World |
| Total Server Accumulated Depreciation | Custom Datacenter |
| Total Server Accumulated Depreciation | Datacenter |
| Total Server Accumulated Depreciation | Cluster Compute Resource |
| Total Server Remaining Depreciation | vSphere World |
| Total Server Remaining Depreciation | Custom Datacenter |
| Total Server Remaining Depreciation | Datacenter |
| Total Server Remaining Depreciation | Cluster Compute Resource |
| VMs Remaining (Average VM Size) | vSphere World |

## Support

This dashboard requires vRealize Operation 8.1 Advanced or Enterprise edition or vRealize Operations Cloud.

Please open an [issue](https://github.com/notoriousbdg/vrops-dashboard-roi/issues) for feedback.

## Changelog
2020-05-20
* Initial release
