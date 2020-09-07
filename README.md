# terraform-aws-asg

This modules creates autoscaling group with ELB too

The required version for this module to work is terraform version 0.11.14

### A sample below is how you can insert the varaibles to use this module

module "asg" {
  
  source  = "ceagone/asg/aws"
  
  version = "1.0.0"
  
  ### #insert the 6 required variables here
  
  desired_capacity = 1
  
  image_owner = "137112412989"
  
  key_name = "bola"
  
  max_size = 1
  
  min_size = 1
  
  region = "us-west-2"
 
}
