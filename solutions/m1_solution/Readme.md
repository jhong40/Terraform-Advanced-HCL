```
cidrsubnet(cidr-range, subnet_bits, network-number) 
cidrsubnet("10.0.0.0/16", 8, 0)   # 1st subnet => 10.0.0.0/24
cidrsubnet("10.0.0.0/16", 8, 1)   # 1st subnet => 10.0.1.0/24

format(spec, values....)
format("%s-%s-vpc", "CompanyA", "Product")  #=> CompanyA-Product-vpc
lower(format("%s-%s-vpc", "CompanyA", "Product"))  # => companya-product-vpc
coalesce("a", "b")    # return the 1st one that is not null # => a
coalesce("","b)       # => b
coalessce(var.owner, var.teamname)    # if owner is define, return it. Otherwise, return teamname
provider::aws::arn_parse(arn)    # break the arn into a map for easy access
```
