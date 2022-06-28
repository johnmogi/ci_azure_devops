# ci_azure_devops

1
how to merge
git push --set-upstream origin 1
=======
check job status
https://dev.azure.com/<organization>/<project>/\_git/<repository>/pullrequest/<pull request id>/timeline

It turned out to be a permission issue to the agent pool. In Organization Settings => Agent Pools => POOL_NAME => Security, there is a setting called Grant access permission to all pipelines. After enabling this, my builds are now working as expected.
