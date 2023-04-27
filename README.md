# TAP GUI Catalog

Sample org structure for application catalog

## Generate Sites for S3:

Reference: https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.4/tap/tap-gui-techdocs-usage.html

For each folder where a `mkdocs.yml` file is present:

```
npx @techdocs/cli generate --source-dir . --output-dir ./site
npx @techdocs/cli publish --publisher-type awsS3 --storage-name <BUCKET_NAME> --entity <NAMESPACE>/<KIND>/<METADATA.NAME> --directory ./site
```



