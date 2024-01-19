# Terraform Local State Move

### Syntax
```bash
./tfmv [include_prefix] [target_state_path] [new_resource_prefix] [plan]
```
* `include_prefix`: The prefix of the resources to be moved in the local state file.
* `target_state_path`: The path for the target local state file.
* `new_resource_prefix`: (Optional) New prefix for the moved resources.
* `plan`: (Optional) If specified, outputs the planned commands without executing.

### Example
```bash
./tfmv module.old target/terraform.tfstate module.new plan
```
