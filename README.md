# Terraform Practice

This repository contains Terraform configurations for learning and practicing Infrastructure as Code (IaC).

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html) >= 1.0
- Cloud provider credentials (AWS, Azure, GCP, etc.)
- Basic understanding of cloud infrastructure concepts

## Getting Started

### Installation

1. Install Terraform following the [official installation guide](https://learn.hashicorp.com/tutorials/terraform/install-cli)
2. Verify installation:
   ```bash
   terraform --version
   ```

### Basic Workflow

1. **Initialize** - Download provider plugins and initialize the working directory:
   ```bash
   terraform init
   ```

2. **Plan** - Preview changes before applying:
   ```bash
   terraform plan
   ```

3. **Apply** - Create or update infrastructure:
   ```bash
   terraform apply
   ```

4. **Destroy** - Remove all infrastructure managed by Terraform:
   ```bash
   terraform destroy
   ```

## Project Structure

```
.
├── modules/          # Reusable Terraform modules
├── environments/     # Environment-specific configurations
│   ├── dev/
│   ├── staging/
│   └── prod/
├── examples/         # Example configurations
└── README.md
```

## Best Practices

- Always run `terraform plan` before `terraform apply`
- Use version control for state files (or remote backends)
- Use variables for reusable values
- Follow naming conventions for resources
- Add meaningful tags to resources
- Document modules and complex configurations
- Use `.gitignore` to exclude sensitive files

## Common Commands

```bash
# Format configuration files
terraform fmt

# Validate configuration
terraform validate

# Show current state
terraform show

# List resources in state
terraform state list

# Output values
terraform output
```

## Resources

- [Terraform Documentation](https://www.terraform.io/docs)
- [Terraform Registry](https://registry.terraform.io/)
- [HashiCorp Learn](https://learn.hashicorp.com/terraform)

## License

This project is for educational purposes.
