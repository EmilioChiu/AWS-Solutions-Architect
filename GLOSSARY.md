# AWS Solutions Architect — Glosario

## A

- **Account ID** — Identificador único de 12 dígitos de una cuenta AWS.
- **ARN (Amazon Resource Name)** — Identificador único para recursos AWS. Formato: `arn:partition:service:region:account:resource`.
- **Availability Zone (AZ)** — Uno o más datacenters discretos dentro de una región. Aislados entre sí en energía, redes y físicamente. Cada región tiene ≥ 2 AZs.
- **AWS CLI** — Herramienta de línea de comandos para interactuar con servicios AWS mediante comandos.
- **AWS Management Console** — Interfaz web para gestionar recursos AWS.
- **AWS SDK** — Bibliotecas específicas por lenguaje de programación para integrar servicios AWS en código.

## C

- **Cloud Computing** — Entrega bajo demanda de recursos de TI (cómputo, almacenamiento, bases de datos) a través de internet con pago por uso.

## E

- **Edge Location** — Sitio de borde de CloudFront para cacheo de contenido. Mínimo 1 por región, pero muchas más a nivel global (~600+).
- **Elastic** — Prefijo que indica que el servicio escala automáticamente (EIP, ELB, EBS, etc.).

## F

- **Free Tier** — Capa gratuita de AWS que incluye ciertos servicios (750h/mes EC2 t2.micro, 5GB S3, etc.) durante los primeros 12 meses + ofertas siempre gratuitas.

## I

- **IaaS (Infrastructure as a Service)** — Provee recursos de infraestructura (VM, storage, redes) bajo demanda. Ej: EC2, S3.
- **PaaS (Platform as a Service)** — Provee plataforma para desplegar código sin gestionar infraestructura subyacente. Ej: Elastic Beanstalk.
- **SaaS (Software as a Service)** — Software completo entregado vía web. Ej: Gmail, Salesforce.

## M

- **MFA (Multi-Factor Authentication)** — Autenticación de múltiples factores (algo que sabes + algo que tienes) para proteger la cuenta.
- **Multi-AZ** — Despliegue en múltiples Availability Zones para alta disponibilidad.

## R

- **Region** — Área geográfica que contiene 2+ Availability Zones. Cada región es completamente independiente (aislamiento de datos, red, servicios).
- **Root User** — Usuario creado al registrar la cuenta. Tiene acceso completo y sin restricciones. No se debe usar para tareas diarias.
