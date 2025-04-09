https://ws001.sspa.juntadeandalucia.es/confluence/pages/viewpage.action?pageId=247564324

# Problemas
Componente de visualización, creación, modificación y eliminación de problemas de enfermería. Un problema siempre estará asociado a un diagnóstico NADA

## Responsabilidad
Según EVS, la responsabilidad del componente debería ser de ECC pero DBS propone y RECOMIENDA que debería de ser su responsabilidad
https://ws001.sspa.juntadeandalucia.es/confluence/pages/viewpage.action?pageId=242167683

## Dudas
- Nos interesa que lo implemente DBS?*

_*Supondría suministrar NANDA. En caso contrario deberíamos de implementar toda la gestión de problemas en un nuevo componente y DBS simplemente usaría nuestro microfrontend_

### Justificación de implementación en ECC
https://chatgpt.com/share/67f63b99-ed54-8013-af92-d959bd2e143b

## EVS
Supone un cambio de alcance

# Hoja de seguimiento de consulta de enfermería
Hoja de seguimiento de consultas requiere integraciones/accesos de varias funcionalidades y módulos. Concretamente a GI, constantes, "sugerencias de cuestionarios y diagnósticos", 
valoración, cuestionarios y agenda

## Responsabilidades
- [GI/ECC?] La propia hoja de seguimiento que integrará constantes
- [DBS/ECC?] Juicios clínicos: que permitirá la selección de diagnósticos y se permitirá mandar al plan y/o asociar a un problema
- [ECC] Sugerencias de cuestionarios y diagnósticos
- [ECC] Valoración inicial
- [ECC] Cuestionarios
- [ECC] Agenda
- [ECC] Plan de cuidados

## Dudas
- Responsabilidad en cuanto a implementación de la propia hoja y juicios clínicos
- Posibilidad de cambio de flujo para eliminar "jucios clinicos" y "sugerencias" y conservar lógica de ECC (menor coste)

## EVS


# Agenda
Componente nuevo con arquitectura de referencia para la gestión de agenda. Requiere hablarse con diagnóstico

## Dudas
- Requiere integración con constantes?

## EVS
Sin cambio de alcance


# ECC - Reutilización
Dudas genéricas
- Debemos seguir el sistema de diseño UX?
- Adaptación para integración?
- Adaptación para el nuevo flujo de autenticación/autorización?
- Producir eventos para navegación?
- Notificar cambio de estado?

## Plan de cuidados
Reutilización del plan de cuidados de ECC

### Adaptación
Requiere configuración y desarrollo del plan de cuidados de hospitalización
https://ws001.sspa.juntadeandalucia.es/confluence/pages/viewpage.action?pageId=240290208

Además, requiere adaptación para el ámbito asitencial de primaria

### PPS
Valorar si requiere optimización a nivel de implementación y/o infraestructura

### Dudas
- 

### EVS
Por confirmar en función de las dudas

## Valoración
Reutilización de valoración inicial de ECC

### Adaptación
Requiere configuración y desarrollo
https://ws001.sspa.juntadeandalucia.es/confluence/pages/viewpage.action?pageId=240290208

### PPS
Valorar si requiere optimización a nivel de implementación y/o infraestructura

### Dudas
- 

# Cuestionarios
Reutilización de cuestionarios de ECC

### Adaptación
Requiere configuración y desarrollo
https://ws001.sspa.juntadeandalucia.es/confluence/pages/viewpage.action?pageId=240290208

### PPS
Valorar si requiere optimización a nivel de implementación y/o infraestructura

### Dudas
- Realmente es necesario pasar por cuestionarios ECC para abrir GI? No debería de abrirse directamente GI?
