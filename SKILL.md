---
name: buscar-contactos-linkedin
description: Encontrar en LinkedIn a las personas a las que el usuario tiene que escribirle (para entrevistas, clientes, alianzas o pedir ayuda) y entregarle por cada una el link al perfil verificado y el mensaje listo para pegar. Usar cuando pida "búscame a quién escribirle", "encuéntrame directores de X", "métete a LinkedIn", "a quién le hablo para esto", o pida revisar a quién volver a escribirle.
---

# Buscar contactos en LinkedIn

El trabajo tiene dos partes. Encontrar a la persona correcta, con el cargo
verificado hoy. Y darle al usuario el mensaje más corto que funcione.

## 1. Antes de buscar

Saca de la conversación o del proyecto, y pregunta solo lo que falte:

- **Para qué.** Entrevista, cliente, alianza, pedir ayuda. Cambia el mensaje.
- **Qué instituciones o tipo de persona.** Si no está claro, propón una lista
  de instituciones con el cargo que buscas en cada una y que el usuario elija.
- **Cuántos.** Por defecto 10 a 15, ordenados por prioridad.
- **Quién es el usuario.** Nombre y organización con que se presenta, para
  firmar el mensaje.
- **Ya contactados.** Busca en el proyecto un archivo de seguimiento de
  contactos (por ejemplo `Seguimiento LinkedIn.md`). Nadie de esa lista ni de
  los descartados vuelve a aparecer.

## 2. Buscar y verificar

1. **Lista de instituciones y cargos.** Primero qué instituciones, después qué
   cargo en cada una tiene la respuesta (director, jefe de innovación,
   coordinador, encargado de emprendimiento, etc.).
2. **Apollo en la web, si el usuario tiene cuenta.** Con la sesión abierta en
   su navegador, el plan gratis permite buscar en la web aunque no por API.
   Armar la búsqueda por URL, por ejemplo
   `https://app.apollo.io/#/people?personLocations[]=Chile&personTitles[]=director%20de%20innovacion`,
   leer el texto de la página y sacar los links de LinkedIn. Solo leer: sin
   "Access email" ni "Access Mobile", que gastan créditos. Si aparece un aviso
   de pago, cerrarlo. Los datos de Apollo pueden estar viejos, así que igual
   se verifica en LinkedIn (paso 3).
   **Si no, LinkedIn directo**, en el navegador con la sesión del usuario:
   `https://www.linkedin.com/search/results/people/?keywords=<cargo + institución>`.
   Si pide iniciar sesión, que lo haga el usuario. Sin navegador, búsqueda web
   con `site:linkedin.com/in`.
3. **Verificar el cargo actual.** Abrir el perfil y confirmar que el cargo
   actual calza con la institución. Es el paso que más falla: resultados de
   buscadores que resultan ser otra persona o alguien que ya se fue. Si no se
   puede confirmar, no va en la lista principal.
4. **Confianza.** Cada persona lleva *alta* (perfil abierto, cargo actual
   calza) o *media* (la web oficial confirma el cargo pero el perfil no se
   pudo abrir; el link es una búsqueda y el usuario elige). Baja no se
   entrega.
5. Con muchas instituciones, repartir en 2 o 3 subagentes por segmento, con
   estas mismas reglas de verificación.

En el navegador solo se lee. Las solicitudes, mensajes e InMails los manda el
usuario.

## 3. Los mensajes

Lo aprendido en tandas reales de contacto:

- **Corto responde más.** Una sola razón para escribir, sin frases que se
  justifican ni promesas de mandar resultados después.
- **Solicitud de conexión con nota** rinde más que el InMail de Sales
  Navigator. Si acepta y no responde, un DM a los 3 o 4 días.
- **La nota tiene máximo 200 caracteres**, contando el nombre ya puesto.
- **Dos días concretos y la duración** (25 minutos, videollamada o llamada).
  Si hay acceso al calendario del usuario, proponer días libres.
- Tuteo o usted según el país y el cargo; sin emojis. Nombre de la persona y
  de su institución siempre puestos en la versión final. Si el usuario tiene
  una guía de voz o una skill de escritura, seguirla.

Plantilla base (adaptar al propósito):

Nota
```
Hola Carolina, soy <tu nombre>, de <tu organización>. Estamos investigando <tema en una línea>. ¿Tendrías 25 minutos el jueves 6 o el martes 11, por videollamada o llamada?
```

DM si acepta y no responde
```
Gracias por aceptar, Carolina. ¿Te acomoda el jueves 6 o el martes 11? Son 25 minutos por videollamada o llamada.
```

## 4. Formato de entrega

En el chat, ordenado por prioridad, una entrada por persona. Cada texto en su
propio bloque de código para que se copie con un clic.

    **1. Nombre Apellido** · Cargo, Institución · confianza alta
    https://www.linkedin.com/in/...

    Nota
    ```
    ...
    ```
    DM si acepta
    ```
    ...
    ```

Si el usuario pide InMail, agregar Asunto e InMail debajo de la nota. Al
final, una línea con los descartados y por qué.

Guardar o actualizar la lista con fecha en el archivo de seguimiento del
proyecto; si no existe, crear `Seguimiento LinkedIn.md`.
