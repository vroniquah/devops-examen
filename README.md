devops-examen
Proyecto Semestral DevOps - Sistema de Ventas y Despachos 

Este repositorio contiene la automatización y despliegue (CI/CD) de una plataforma de ventas y despachos, desarrollado como Evaluación Final Transversal para la asignatura Introducción a Herramientas DevOps.

Tecnologías Utilizadas
Frontend: React.js (Nginx)
 Backend (Microservicios): Java Spring Boot
Base de Datos:PostgreSQL
Contenedores: Docker y Docker Compose
CI/CD: GitHub Actions
Cloud: AWS (ECR, ECS Fargate, VPC)

Arquitectura Cloud y Pipeline
1. GitHub Actions: Automatiza el build de las imágenes Docker de los 3 componentes (Frontend, API Ventas, API Despachos).
2. Amazon ECR: Almacena de forma privada las imágenes generadas.
3. Amazon ECS (Fargate): Orquesta los contenedores en producción asegurando alta disponibilidad, sin necesidad de administrar servidores (Serverless).

Autor
Veronica Ávila
