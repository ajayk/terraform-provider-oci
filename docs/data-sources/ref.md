---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "oci_ref Data Source - terraform-provider-oci"
subcategory: ""
description: |-
  Image ref data source
---

# oci_ref (Data Source)

Image ref data source



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `ref` (String) Image ref to lookup

### Read-Only

- `config` (Object) Config of an image. (see [below for nested schema](#nestedatt--config))
- `digest` (String) Image digest of the image.
- `id` (String) Fully qualified image digest of the image.
- `images` (Map of Object) Map of image platforms to manifests. (see [below for nested schema](#nestedatt--images))
- `manifest` (Object) Manifest of the image or index. (see [below for nested schema](#nestedatt--manifest))
- `tag` (String) Image tag of the image.

<a id="nestedatt--config"></a>
### Nested Schema for `config`

Read-Only:

- `cmd` (List of String)
- `created_at` (String)
- `entrypoint` (List of String)
- `env` (List of String)
- `user` (String)
- `working_dir` (String)


<a id="nestedatt--images"></a>
### Nested Schema for `images`

Read-Only:

- `digest` (String)
- `image_ref` (String)


<a id="nestedatt--manifest"></a>
### Nested Schema for `manifest`

Read-Only:

- `annotations` (Map of String)
- `config` (Object) (see [below for nested schema](#nestedobjatt--manifest--config))
- `layers` (List of Object) (see [below for nested schema](#nestedobjatt--manifest--layers))
- `manifests` (List of Object) (see [below for nested schema](#nestedobjatt--manifest--manifests))
- `media_type` (String)
- `schema_version` (Number)
- `subject` (Object) (see [below for nested schema](#nestedobjatt--manifest--subject))

<a id="nestedobjatt--manifest--config"></a>
### Nested Schema for `manifest.config`

Read-Only:

- `digest` (String)
- `media_type` (String)
- `platform` (Object) (see [below for nested schema](#nestedobjatt--manifest--config--platform))
- `size` (Number)

<a id="nestedobjatt--manifest--config--platform"></a>
### Nested Schema for `manifest.config.platform`

Read-Only:

- `architecture` (String)
- `os` (String)
- `os_version` (String)
- `variant` (String)



<a id="nestedobjatt--manifest--layers"></a>
### Nested Schema for `manifest.layers`

Read-Only:

- `digest` (String)
- `media_type` (String)
- `platform` (Object) (see [below for nested schema](#nestedobjatt--manifest--layers--platform))
- `size` (Number)

<a id="nestedobjatt--manifest--layers--platform"></a>
### Nested Schema for `manifest.layers.platform`

Read-Only:

- `architecture` (String)
- `os` (String)
- `os_version` (String)
- `variant` (String)



<a id="nestedobjatt--manifest--manifests"></a>
### Nested Schema for `manifest.manifests`

Read-Only:

- `digest` (String)
- `media_type` (String)
- `platform` (Object) (see [below for nested schema](#nestedobjatt--manifest--manifests--platform))
- `size` (Number)

<a id="nestedobjatt--manifest--manifests--platform"></a>
### Nested Schema for `manifest.manifests.platform`

Read-Only:

- `architecture` (String)
- `os` (String)
- `os_version` (String)
- `variant` (String)



<a id="nestedobjatt--manifest--subject"></a>
### Nested Schema for `manifest.subject`

Read-Only:

- `digest` (String)
- `media_type` (String)
- `platform` (Object) (see [below for nested schema](#nestedobjatt--manifest--subject--platform))
- `size` (Number)

<a id="nestedobjatt--manifest--subject--platform"></a>
### Nested Schema for `manifest.subject.platform`

Read-Only:

- `architecture` (String)
- `os` (String)
- `os_version` (String)
- `variant` (String)


