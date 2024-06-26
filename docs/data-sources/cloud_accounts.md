---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "tdh_cloud_accounts Data Source - tdh"
subcategory: ""
description: |-
  Used to fetch all cloud accounts on TDH.
  Note: For SRE only.
---

# tdh_cloud_accounts (Data Source)

Used to fetch all cloud accounts on TDH.
**Note:** For SRE only.

## Example Usage

```terraform
data "tdh_cloud_accounts" "all" {
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `list` (Attributes List) (see [below for nested schema](#nestedatt--list))

### Read-Only

- `id` (String) The testing framework requires an id attribute to be present in every data source and resource

<a id="nestedatt--list"></a>
### Nested Schema for `list`

Read-Only:

- `created_at` (String) Creation time of this account.
- `created_by` (String) User which created this account.
- `data_plane_count` (Number) Total data planes associated with this account.
- `id` (String) ID of the cloud account.
- `management_ip` (String) IP of the management console.
- `modified_at` (String) Last time this account was modified.
- `modified_by` (String) User which last modified this account.
- `name` (String) Name of the cloud account.
- `org_id` (String) OrgId of the cloud account
- `provider_type` (String) Account type of the cloud account
- `shared` (Boolean) Whether this account is shared between multiple Organisations or not.
- `tags` (Set of String) Tags set on this account.
- `user_email` (String) User email of the cloud account


