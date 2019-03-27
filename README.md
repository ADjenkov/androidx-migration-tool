Tool that migrates Support Library namespaces to the new AndroidX namespaces.

It searches recursively .java,.js,.ts,.xml and .gradle files.

How to use:
  1. `npm install`
  2. `npm run migrate-namespaces test-plugin` (where `test-plugin` should be your project folder)
      This command will search and replace all Support Library namespace to the new AndroidX namespaces
      Please do revise all changes manually after that!
      This operation may take a few minutes to execute (depends on your project structure size).
  3.  `npm run migrate-artifacts test-plugin` (where `test-plugin` should be your project folder)
      This command will output suggestions, that should be made manually, for changing Support Library artifacts to AndroidX.

This tool does not migrate any 3rd party packages or plugins that your project relies on. 
Consider updating your project `package.json` dependencies with AndroidX versions.

Demo `test-plugin` included.
