# Propuesta: Sistema de Firma Digital de NEPs

Landing page profesional para la propuesta técnica de implementación de un sistema de firma digital para Notas de Encargo Programadas (NEPs).

## 📋 Contexto

- **Cliente:** Empresa de Ley de Segunda Oportunidad
- **Volumen:** 30-60 NEPs/mes
- **Solución:** Firma digital con OTP por SMS mediante DocuSeal + LabsMobile
- **Integración:** Sistema legacy Zunzun (VB + SQL Server)

## 🎯 Objetivo

Transformar el proceso actual de firma en papel a un flujo digital completo:
1. Generación digital del NEP
2. Envío al firmante vía email/SMS
3. Firma con código OTP verificado
4. Almacenamiento seguro con trazabilidad

## 🛠️ Stack Tecnológico

- **DocuSeal:** Firma digital open source
- **FastAPI:** API bridge y backend
- **React:** Dashboard administrativo
- **SQL Server:** Base de datos existente
- **LabsMobile:** OTP por SMS
- **Docker:** Containerización
- **Nginx:** Proxy inverso y SSL

## 📐 Arquitectura

```
Zunzun → API Bridge → DocuSeal → OTP SMS → Almacenamiento
            ↓
        Dashboard React
```

## ⏱️ Timeline

- **Fase 1 (Semana 1):** Análisis y setup
- **Fase 2 (Semana 1-2):** Integración Zunzun → DocuSeal
- **Fase 3 (Semana 2-3):** OTP y flujo de firma
- **Fase 4 (Semana 3):** MVP en producción
- **Fase 5 (Semana 4-5):** Dashboard y robustecimiento

## 🚀 Despliegue

Esta landing está desplegada en GitHub Pages:

**URL:** https://weavewes.github.io/proposal-nep-firma-digital/

## 📁 Estructura

```
.
├── index.html      # Landing page principal (SPA)
└── README.md       # Este archivo
```

La landing es un single-file HTML con CSS y JavaScript inline para facilitar el despliegue en GitHub Pages sin dependencias externas (salvo fuentes e iconos vía CDN).

## 🎨 Diseño

- **Colores:** Paleta Weaves (#1c1c1c, #f7f4ed, #eceae4)
- **Tipografía:** Playfair Display + Inter
- **Iconos:** Lucide (CDN)
- **Responsive:** Desktop y móvil

---

*Propuesta técnica preparada por Weaves · 2025*
