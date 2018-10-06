## SETUP

Boilerplate based on a blog project.

### resources.yml

Naming of various resource/policies/roles of AWS resources follow the format `<PROJECTNAME><env><ResourceName>`.
* No spacing allowed
* Multiple projects of multiple environment will share the same AWS account for some resources, so need to differentiate each resource by project name and environment.
* `env` is lowercased so that interpolation in `serverless.yml` do not require manipulation. Is this even possible?