
# Grafana Dashboard Automation Framework using postman scripting with Javascript

Tools and Technologies

* Postman
* Javascript
* Newman

## Product domain initialization

* Change domain name from environment json file
* Install newman using nodejs 

```bash
npm install -g newman
```
      
## Execute postman script collection file from newman

Execute following command from the relavent file location 

```bash
newman run Grafana-Promethus-Automation.postman_collection.json -e Prometheus-Env.postman_environment.json --insecure
```

* To get the Newman advance report

```bash
npm install -g newman-reporter-htmlextra
```

```bash
newman run Grafana-Promethus-Automation.postman_collection.json -e Prometheus-Env.postman_environment.json -r htmlextra Grafana-Newman-Report.html --insecure
```

![Logo](https://axiatadigitallabssl-my.sharepoint.com/:i:/r/personal/vikum_sugathadasa_axiatadigitallabs_com/Documents/Attachments/Newman-Report01.PNG?csf=1&web=1&e=jqz6Py)

