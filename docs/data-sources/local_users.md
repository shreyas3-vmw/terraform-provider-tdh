---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "tdh_local_users Data Source - tdh"
subcategory: ""
description: |-
  Used to fetch local users present on TDH.
---

# tdh_local_users (Data Source)

Used to fetch local users present on TDH.

## Example Usage

```terraform
data "tdh_local_users" "by_username" {
  username = "some_username"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `username` (String) Name of the local user to filter results by.

### Read-Only

- `id` (String) ID of the task.
- `list` (Attributes List) List of local users. (see [below for nested schema](#nestedatt--list))

<a id="nestedatt--list"></a>
### Nested Schema for `list`

Read-Only:

- `id` (String) ID of the task.
- `policy_ids` (Set of String) IDs of the policies attached to this local user.
- `username` (String) Name of the local user.

