- ECC evolución primaria vs nueva aplicación
-- EVOLUCIÓN
--- Existe gran cantidad de requerimientos funcionales compartidos
--- Mantener una única base facilitaría la transición y reduciría deuda técnica
--- Reduce el coste gestión y mantenimiento
--- Aumentaría la complejidad

-- NUEVA
--- Reduce complejidad
--- Libertad evolución con requisitos específicos por ámbito
--- Reduce riesgo de falla por features de otro ámbito

- Estandarización integración frontal
-- Actualmente, para microfrontales, usamos app-shell con capabilities de aislamiento o integración directa pero este está acoplado a Lit
-- Posibilidad de plantear un componente similiar para estandarizar apps legacy y establecer comunicación entre iframe de forma transparente
-- Evitamos la responsabilidad del host de crear un iframe y establecer la comunicación con este
-- Evaluar otros módulos para el estudio de su viabilidad
-- Estandarización de propiedades y eventos
-- Definición de navegadores soportados
-- Definición de otros requisitos/limitaciones del cliente

- Pruebas de carga inicial
-- Anticiparnos a posibles fallas de rendimiento al someter a ECC a un mayor estrés
-- La solución de estos problemas, podrían requeririr optimizaciones software y/o hardware
-- Para ello necesitamos:
--- Volumetria (pendiente de solicitarlo hsap):
--- Definición arquitectónica
--- DGT y entorno de pruebas PRE/DEV
--- Configuración entornuo

- Análisis implicaciones centralización

- Análisis implicaciones cambio de ámbito

--- 8/5/2025

Implicaciones de reutilizar ECCWeb
Inconvenientes
- Solo reutilizaremos una funcionalidad (plan de cuidados)
- Adaptación para la centralización
- Adaptación para el cambio de ámbito
- Adaptador para comunicación por eventos en weblogic
- Optimización rendimiento / refactor
- Adaptación al sistema de diseño actual
- Adaptación del propio plan de cuidados
- Complejidad añadida al mantener dos ámbitos
- ADR integración frontales legacy

PPS
- Aprovechar para testar la versión de ECC

-- 14/05/2025
Requisito RF-016 El historico lo mantenemos en plan de cuidados con borrado lógico o lo pasamos a auditoría con borrado físico en plan de cuidados?
Requisito RF-035 Si recomendaciones necesita poder seleccionar cualquier etiqueta aunque no esté sugerida, necesita todas las etiquetas que están en plan. Duplicamos info o creamos un servicio unificado?






