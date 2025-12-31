# Hoja de Trabajo: Análisis de Fuga de Datos

Este documento detalla el análisis del incidente de seguridad y las recomendaciones aplicadas bajo el estándar NIST.

| Sección | Descripción y Análisis |
| :--- | :--- |
| **Control** | **Mínimo privilegio (Least privilege)** |
| **Problema(s)** | La filtración ocurrió porque el gerente otorgó acceso excesivo a una carpeta con documentos internos altamente sensibles sin revocarlo tras la reunión. Además, la falta de una separación clara entre materiales públicos y privados permitió que un empleado compartiera accidentalmente el enlace incorrecto por error humano. |
| **Revisión** | El control **NIST SP 800-53: AC-6** se refiere al principio de mínimo privilegio, el cual exige que a los usuarios se les otorguen solo los derechos de acceso necesarios para realizar sus funciones. Este control busca limitar el daño potencial de errores accidentales o acciones malintencionadas mediante la restricción estricta de permisos. |
| **Recomendación(es)** | 1. Implementar un sistema de **Control de Acceso Basado en Roles (RBAC)** que separe estrictamente los materiales de marketing públicos de la propiedad intelectual interna. <br> 2. Configurar **permisos temporales o de caducidad automática** para carpetas compartidas en reuniones, asegurando que el acceso se revoque sin intervención manual. |
| **Justificación** | Estas mejoras abordan el problema de raíz al reducir la superficie de exposición de los datos. Al automatizar la revocación y organizar los archivos por nivel de sensibilidad, se minimiza la probabilidad de que un error individual de un empleado resulte en la divulgación de secretos comerciales de la empresa. |

---
*Análisis realizado como parte de la formación en Ciberseguridad de Google.*
