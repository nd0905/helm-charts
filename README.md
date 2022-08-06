# helm-charts
A place to hold and build all my used helm charts


## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:
```
helm repo add nd0905 https://nd0905.com/helm-charts
```
If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
nd0905` to see the charts.

To install the <chart-name> chart:
```
helm install <chart-name> nd0905/<chart-name>
```
To uninstall the chart:
```
helm delete <chart-name>
```
