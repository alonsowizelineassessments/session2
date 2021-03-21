# Wizeline Session 2

Postman and Newman

### Postman Collection 🚀

todoist.json

### Installation 🔧

```bash
npm install -g newman
npm install -g newman-reporter-htmlextra
```

### Pre-requistes to run in CI/CD pipeline 
_Make sure to set your API token in an environment variable_

* **UNIX** - *Add TOKEN in your enviroment variables (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc)" export TOKEN="1328006e5c8ee887807ba4d2cec8bef27127e712"*
* **WINDOWS** - *Add TOKEN in your enviroment variables (System env variables)"*

### Newman run from CLI

```bash
newman run todoist.json -r cli,htmlextra -d data/data.json --global-var TOKEN=$TOKEN
```

### Running in Postman
Update Collection Authorization Token, with your todist API token
