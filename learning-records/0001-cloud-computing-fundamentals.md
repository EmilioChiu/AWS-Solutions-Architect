# ADR 0001: Cloud Computing & AWS Global Infrastructure

**Date:** 2026-06-26
**Session:** 1/50
**Milestone:** w1d1

## What I Learned

- Cloud computing: entrega bajo demanda de recursos TI con pago por uso.
- Modelos: IaaS (control total, ej: EC2), PaaS (solo código, ej: Elastic Beanstalk), SaaS (app completa, ej: Gmail).
- Ventajas clave: elasticidad, pago por uso, alcance global, no adivinar capacidad.
- Infraestructura AWS: Regions (≥2 AZs) → Availability Zones (datacenters aislados) → Edge Locations (caching CDN).
- Multi-AZ = mínimo para alta disponibilidad.
- Factores para elegir región: latencia, cumplimiento, costo, disponibilidad de servicios.
- Servicios globales (IAM, Route 53, CloudFront) vs regionales (EC2, RDS, Lambda, S3).
- AWS CLI: interfaz de línea de comandos para interactuar con servicios AWS.
- AWS Management Console: interfaz web para gestionar recursos.
- Free Tier: capa gratuita (750h/mes EC2 t2.micro, 5GB S3, etc.) primeros 12 meses.
- Seguridad: MFA obligatorio en cuenta root, crear usuario IAM para uso diario.
- ARN: identificador único de recursos AWS.

## Key Insights

- **Infraestructura programable:** AWS no es un datacenter tradicional — todo se controla por API. Como backend dev, esto es natural: tratas infraestructura como código.
- **Multi-AZ no es opcional:** Para producción, siempre mínimo 2 AZs. Es la línea entre app disponible y app caída.
- **Root user = arma nuclear:** Solo para facturación y cambios críticos. El día a día se hace con usuarios IAM.
- **Regiones son soberanas:** Los datos no cruzan regiones a menos que explícitamente configures cross-region replication.

## Skills Acquired

- [x] Crear cuenta AWS Free Tier
- [x] Habilitar MFA en cuenta root
- [x] Crear usuario IAM administrador
- [x] Navegar AWS Management Console
- [x] Instalar y configurar AWS CLI
- [x] Ejecutar comandos CLI (`aws ec2 describe-regions`)

## Questions / Uncertainties

- Queda pendiente entender en detalle la diferencia entre servicios globales y regionales (¿S3 es regional o global? Los buckets son globales pero los datos son regionales).
- ¿Cómo funciona el facturador cuando un recurso vive en múltiples regiones?

## Next

- Próximo: w1d2 — Pricing, Facturación & Soporte
