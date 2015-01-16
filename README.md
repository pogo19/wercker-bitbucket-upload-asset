bitbucket-upload-asset-wildcard
===============================

Upload specified file(s) to repository's Downloads on bitbucket.
Allows wildcards in 'file' parameter, e.g. target/*.war.

Use in your `wercker.yml` in this way:
    steps:
        - pogo/bitbucket-upload-asset-wildcard@0.0.2:
            username: ${BITBUCKET_USERNAME}
            password: ${BITBUCKET_PASSWORD}
            file: target/*.war

Those `BITBUCKET_USERNAME` and `BITBUCKET_PASSWORD` variables need to
be defined in deploy target or pipeline variables.
