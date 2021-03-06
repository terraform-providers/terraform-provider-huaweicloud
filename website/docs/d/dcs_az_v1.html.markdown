---
layout: "huaweicloud"
page_title: "Huaweicloud: huaweicloud_dcs_az_v1"
sidebar_current: "docs-huaweicloud-datasource-dcs-az-v1"
description: |-
  Get information on an Huaweicloud dcs az.
---

# huaweicloud\_dcs\_az_v1

Use this data source to get the ID of an available Huaweicloud dcs az.

## Example Usage

```hcl

data "huaweicloud_dcs_az_v1" "az1" {
  name = "AZ1"
  port = "8004"
  code = "cn-north-1a"
}
```

## Argument Reference

For details, See [Querying AZ Information](https://support.huaweicloud.com/en-us/api-dcs/dcs-api-0312039.html).

* `name` - (Optional) Indicates the name of an AZ.

* `code` - (Optional) Indicates the code of an AZ.

* `port` - (Optional) Indicates the port number of an AZ.


## Attributes Reference

`id` is set to the ID of the found az. In addition, the following attributes
are exported:

* `name` - See Argument Reference above.
* `code` - See Argument Reference above.
* `port` - See Argument Reference above.
