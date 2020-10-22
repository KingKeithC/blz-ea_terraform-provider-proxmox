---
layout: page
title: Datastores
permalink: /data-sources/datastores
nav_order: 1
parent: Data Sources
---

# Data Source: Datastores

Retrieves information about all the datastores available to a specific node.

## Example Usage

```
data "proxmox_virtual_environment_datastores" "first_node" {
  node_name = "first-node"
}
```

## Arguments Reference

* `node_name` - (Required) A node name.

## Attributes Reference

* `active` - Whether the datastore is active.
* `content_types` - The allowed content types.
* `datastore_ids` - The datastore identifiers.
* `enabled` - Whether the datastore is enabled.
* `shared` - Whether the datastore is shared.
* `space_available` - The available space in bytes.
* `space_total` - The total space in bytes.
* `space_used` - The used space in bytes.
* `types` - The storage types.
