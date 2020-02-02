## alfred-workflow-nodejs-template

### For Developtment

#### Prepare

1. Create a new blank Alfred workflow.

2. Add a Script Filter (right-click the canvas → Inputs → Script Filter), set Language to /bin/bash, and add the following script:

```sh
./node_modules/.bin/run-node index.js "$1"
```

3. Open workflow directory and import this repository.

```sh
cd $WORKFLOW_REPOSITORY
git init
git remote add origin https://github.com/SamVerschueren/generator-alfred
git fetch
git pull origin master
npm install
```

#### Release

Export for `.alfredworkflow` from Alfred Preference.
