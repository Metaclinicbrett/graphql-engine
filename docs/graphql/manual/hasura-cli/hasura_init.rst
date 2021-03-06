.. meta::
   :description: Use hasura init to initialise a directory for Hasura migrations on the Hasura CLI
   :keywords: hasura, docs, CLI, hasura init

.. _hasura_init:

Hasura CLI: hasura init
-----------------------

Initialize a directory for Hasura GraphQL engine migrations.

Synopsis
~~~~~~~~


Create directories and files required for enabling migrations on the Hasura GraphQL engine.

::

  hasura init [directory-name] [flags]

Examples
~~~~~~~~

::

    # Create a directory to store migrations
    hasura init [directory-name]

    # Now, edit <my-directory>/config.yaml to add endpoint and admin secret

    # Create a directory with endpoint and admin secret configured:
    hasura init <my-project> --endpoint https://my-graphql-engine.com --admin-secret adminsecretkey

    # See https://hasura.io/docs/1.0/graphql/manual/migrations/index.html for more details

Options
~~~~~~~

::

      --action-handler-webhook-baseurl string   webhook baseurl to be used for an action (default "http://localhost:3000")
      --action-kind string                      kind to be used for an action (default "synchronous")
      --admin-secret string                     admin secret for Hasura GraphQL engine
      --endpoint string                         http(s) endpoint for Hasura GraphQL engine
  -h, --help                                    help for init
      --install-manifest string                 install manifest to be cloned
      --metadata-directory string               name of directory where metadata files will be created (default "metadata")
      --version string                          config version to be used (default "2")

Options inherited from parent commands
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

::

      --log-level string    log level (DEBUG, INFO, WARN, ERROR, FATAL) (default "INFO")
      --no-color            do not colorize output (default: false)
      --project string      directory where commands are executed (default: current dir)
      --skip-update-check   skip automatic update check on command execution

SEE ALSO
~~~~~~~~

* :ref:`hasura <hasura>` 	 - Hasura GraphQL engine command line tool

*Auto generated by spf13/cobra*
