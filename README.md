
# A sample terraform configuration to demonstrate usage of "output" 

### Benefits
By using `"output"` we can get summarised resource details easily visible in the terminal. There is no need to dig in the state file for this information.
The output information will be printed out in the terminal after ``` terraform plan ``` or ```terraform apply```.

### Use Case
In this particular example we create 3 ec2 intances and to follow the best practices we add names for each of them by using `"tags"`. By adding `"output"` block we will get a list with all the names of these ec2 instances.

### Prerequisites
- Git
- Terraform CLI
- AWS credentials

### Repo location
https://github.com/GitHuberkata/output.git

### Result
After applying the code the result in the terminal will look as follows:

```
ec2_names_list = [
  tomap({
    "Name" = "OutputTaskMachine-0"
  }),
  tomap({
    "Name" = "OutputTaskMachine-1"
  }),
  tomap({
    "Name" = "OutputTaskMachine-2"
  }),
]
```
