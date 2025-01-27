---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "oci_append Resource - terraform-provider-oci"
subcategory: ""
description: |-
  Append layers to an existing image.
---

# oci_append (Resource)

Append layers to an existing image.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `layers` (Attributes List) Layers to append to the base image. (see [below for nested schema](#nestedatt--layers))

### Optional

- `base_image` (String) Base image to append layers to.

### Read-Only

- `id` (String) The resulting fully-qualified digest (e.g. {repo}@sha256:deadbeef).
- `image_ref` (String) The resulting fully-qualified digest (e.g. {repo}@sha256:deadbeef).

<a id="nestedatt--layers"></a>
### Nested Schema for `layers`

Required:

- `files` (Attributes Map) Files to add to the layer. (see [below for nested schema](#nestedatt--layers--files))

<a id="nestedatt--layers--files"></a>
### Nested Schema for `layers.files`

Required:

- `contents` (String) Content of the file.


