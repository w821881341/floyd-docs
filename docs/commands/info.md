View the details of a job.

### Usage
```bash
floyd info [OPTIONS] ID
```

### Options
| Name, shorthand | Default | Description |
| --------------- | ------- | ----------- |
| ID |      | ID of your job. You can get the ID by running the [status](./status) command.    |

### Description
This command gives detailed information about your job. Some useful information here:

#### Output ID
Output ID is the reference to the output generated by your run. If you want to use this as the 
input for your next job, use this ID and pass it as `--data ID` in the [run](./run) command.

#### Url
If your job is running in [jupyter](../guides/jupyter) or [serve](../guides/style_transfer/#serve-mode) mode, you can get their URL here.

### Example
```bash
$ floyd info Faa2xpokjAfJL5Jd7vCVXo
-----------  ----------------------------------------------------
Run ID       Faa2xpokjAfJL5Jd7vCVXo
Name         floydhub/jupyter-notebook:1
Created      2 minutes ago
Status       running
Duration(s)  0
Output ID    VB9bF6vtyvrHLdUsFbUuvW
Instance     cpu
Version      1
Mode         jupyter
Url          https://www.floydhub.com:8000/VB9bF6vtyvrHLdUsFbUuvW
-----------  ----------------------------------------------------
```
