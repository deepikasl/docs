page_main_title: GitHub Enterprise
main_section: Platform
sub_section: Integrations
page_title: GitHub Enterprise integration

# GitHub Enterprise Integration

Available under the Integration Family: **SCM**

`Github Enterprise` Integration is used to connect Shippable DevOps Assembly Lines platform to your instance of Github Enterprise Server. 

You can create this from the integrations page. This is the information you would require to create this integration

* **Name** -- friendly name for the integration
* **URL** -- location of your GHE server API. The format is in `https://(Github Enterprise URL)/api/v3`
* **Token** -- personal access token with the right levels of permission

## Resources that use this Integration
Resources are the bulding blocks of assembly lines and some types of resource refer to Integrations by their name. The following Resources Types can created with `Github Enterprise` Integration 

* [gitRepo]()
* [ciRepo]()
* [syncRepo]()

## Default Environment Variables
When you create a Resource with this integration, and use it as an `IN` or `OUT` into a Job that can execute user defined scripts, a set of environment variables are configured by the platform that may be useful to set the context before user defined scripts execute as part of the Job. These are variables available when this Resource is used

`<NAME>` is the the friendly name of the Resource

| Environment variable						| Description                         |
| ------------- 								|------------------------------------ |
| `<NAME>`\_INTEGRATION\_URL    			| Github Enterprise API location |
| `<NAME>`\_INTEGRATION\_TOKEN			| The Token used to connect to Github Enterprise |

## Further Reading
* GKE integration
* AWS integration
* runSH job
* runCLI job
* runCI job
* How to setup CI for my git repo

## TODO
| Tasks   |      Status    |
|----------|-------------|
| Hotlinking |  Open |
| Further Reading needs thinking|  Open |