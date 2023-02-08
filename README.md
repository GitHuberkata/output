
# A sample terraform configuration to demonstrate usage of "output" to printout in the terminal summary of desired resource details in plain text

### Prerequisites

### Benefits
Summarised information is easily accessible/visible in the terminal after the resources are built. There is no need to dig in the state file.
The output information is also visible also when only performing ``` terraform plan ```

Result
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
