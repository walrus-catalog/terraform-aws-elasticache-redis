# Replication Example

Deploy Redis service in standalone architecture by root module.

```bash
# setup infra
$ terraform apply -auto-approve \
  -target=aws_vpc.example \
  -target=aws_subnet.example \
  -target=aws_kms_key.example \
  -target=aws_service_discovery_private_dns_namespace.example

# create service
$ terraform apply -auto-approve
```

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 5.24.0 |
| <a name="requirement_random"></a> [random](#requirement\_random) | >= 3.5.1 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 5.24.0 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_this"></a> [this](#module\_this) | ../.. | n/a |

## Resources

| Name | Type |
|------|------|
| [aws_kms_key.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/kms_key) | resource |
| [aws_service_discovery_private_dns_namespace.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/service_discovery_private_dns_namespace) | resource |
| [aws_subnet.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.example](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |
| [aws_availability_zones.selected](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_address"></a> [address](#output\_address) | n/a |
| <a name="output_address_readonly"></a> [address\_readonly](#output\_address\_readonly) | n/a |
| <a name="output_connection"></a> [connection](#output\_connection) | n/a |
| <a name="output_connection_readonly"></a> [connection\_readonly](#output\_connection\_readonly) | n/a |
| <a name="output_context"></a> [context](#output\_context) | n/a |
| <a name="output_password"></a> [password](#output\_password) | n/a |
| <a name="output_port"></a> [port](#output\_port) | n/a |
| <a name="output_refer"></a> [refer](#output\_refer) | n/a |
<!-- END_TF_DOCS -->