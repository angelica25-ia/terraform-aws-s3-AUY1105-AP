# Terraform AWS S3 Module

Módulo Terraform reutilizable para la creación de buckets S3 en AWS.

---

# Objetivo

Este módulo permite desplegar recursos de almacenamiento en AWS utilizando Terraform y buenas prácticas de infraestructura modular.

---

# Recursos Implementados

- AWS S3 Bucket reutilizable

---

# Variables

| Variable | Descripción |
|---|---|
| bucket_name | Nombre del bucket |
| environment | Nombre del entorno |

---

# Outputs

| Output | Descripción |
|---|---|
| bucket_name | Nombre del bucket |
| bucket_arn | ARN del bucket |

---

# Uso del módulo

```hcl
module "storage" {
  source = "git::https://github.com/angelica25-ia/terraform-aws-s3-AUY1105-AP.git"

  bucket_name = "my-terraform-bucket"
  environment = "dev"
}

Requisitos
Terraform >= 1.0
AWS Provider >= 5.0

Autor
Angelica Poblete