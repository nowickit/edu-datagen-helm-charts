These are the helm charts to build the edu datagen for Kubernetes and kube-related courses.
There is a github action to automatically build the helm chart repo located at
https://splunk.github.io/edu-datagen-helm-charts/, any time the charts are changed

**Note that the chart repo artifacts may expire if not used for 90 days.**

You can force a rebuild of the artifacts by editing the chart file at:
    charts/splunk-k8s-o11y-datagen/Chart.yaml
You must update the version number on line 18 of the above file.
When you commit the change to the repo, it will trigger rebuilding the artifacts and chart repo.

Note that if you make any changes to the charts, you must also update the version number as noted above so that the change is pushed to the artifact repo.
