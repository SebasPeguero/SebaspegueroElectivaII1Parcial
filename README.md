# 1er Parcial: Integración Continua con Surge.sh y GitHub Actions

**Estudiante:** Sebastián Peguero  
**Matrícula:** 2025-1172  
**Materia:** Electiva II (DevOps)  
**Institución:** Instituto Tecnológico de Las Américas (ITLA)  
**Repositorio:** [SebaspegueroElectivaII1Parcial](https://github.com/SebasPeguero/SebaspegueroElectivaII1Parcial)  
**URL de la Página en Surge.sh:** [https://sebaspegueroelectivaii1parcial.surge.sh](https://sebaspegueroelectivaii1parcial.surge.sh)

---

## 🎯 Objetivo de la Práctica
Crear un repositorio local de Git con una página web en HTML y configurar un pipeline de Integración Continua (CI) mediante **GitHub Actions** para que, al realizar un `push` a la rama `main`, la página se despliegue automáticamente en **Surge.sh**.

## 🔒 Gestión Segura de Credenciales (GitHub Secrets)
Para no exponer la clave de Surge públicamente en el repositorio:
* Se configuró el secreto `SURGE_LOGIN` con el correo de autenticación.
* Se configuró el secreto `SURGE_TOKEN` con el token de acceso de Surge.
* El archivo `.github/workflows/main.yaml` referencia estos secretos de forma segura mediante `${{ secrets.SURGE_TOKEN }}` y `${{ secrets.SURGE_LOGIN }}`.

## 📁 Estructura del Repositorio
* `index.html`: Página web desarrollada para el 1er Parcial.
* `.github/workflows/main.yaml`: Flujo de trabajo de GitHub Actions para el despliegue automático en Surge.sh.
* `README.md`: Documentación general del proyecto.
