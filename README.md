# Route Table Module
Whats is the route table module? This module creates route tables.

How to use the route table module? 
This module was created with list of strings to use for specification of the route table parameters

outputs:

route table : id of the created route table

To use this kind of variable in the module it's necessary create a instance of the variable on de main.tf, for example:

module "subnet" {<br>
  source = "git::https://github.com/BrunoHigino06/aws_route_table_module.git"<br>
<br>
  rt_names = ["Private", "Public"]<br>
}
