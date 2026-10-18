# Seguridad

Centralita CRM está diseñada para que **los datos de tus clientes solo puedan leerse en los teléfonos que tu empresa ha autorizado**. Ni el servidor de distribución ni la red pueden leerlos.

## Garantías

| Garantía | Qué significa para ti |
| --- | --- |
| Cifrado de extremo a extremo | Los datos se cifran en origen para cada teléfono autorizado; el servidor solo almacena información cifrada |
| Una clave por teléfono | Cada terminal genera sus propias claves; la clave privada nunca sale del dispositivo |
| Firma digital de cada paquete | El teléfono rechaza cualquier dato alterado o no emitido por tu empresa |
| Emisor fijado en la app | La app solo acepta datos firmados por la clave de tu empresa, nunca por una clave recibida junto a los datos |
| Descargas autenticadas | Cada petición del teléfono va firmada, con caducidad temporal y protección frente a repeticiones |
| Sin retrocesos de versión | El teléfono rechaza versiones de datos antiguas |
| Transporte protegido | Solo HTTPS, con certificados del servidor fijados en la app (*certificate pinning*) |
| Almacenamiento cifrado | La caché local y los datos de identificación de llamadas se cifran con claves protegidas por el hardware del teléfono |
| Sin copias de seguridad | Los datos de la app se excluyen de las copias en la nube y de la transferencia entre dispositivos |
| Revocación | Al bloquear un terminal, este borra sus datos en el siguiente contacto |
| Caducidad sin conexión | Los datos locales dejan de mostrarse si el teléfono pasa demasiado tiempo sin sincronizar |

## Algoritmos

Se utilizan algoritmos estándar y ampliamente auditados:

- **Cifrado de datos:** AES-256-GCM.
- **Intercambio de claves:** X25519 con derivación HKDF-SHA256.
- **Firmas:** Ed25519.
- **Integridad:** SHA-256.

## Qué no cubre

Ser transparentes sobre los límites también forma parte de la seguridad:

- Un teléfono comprometido (con *root* o malware con privilegios) puede ver los datos que la app muestra en pantalla.
- Quien tenga el teléfono desbloqueado verá lo mismo que su usuario legítimo; protege el dispositivo con bloqueo de pantalla.
- La aprobación de terminales es una decisión de tu administrador: aprueba solo los dispositivos que reconozcas.

## Buenas prácticas recomendadas

- Activa el bloqueo de pantalla y el cifrado del dispositivo.
- Revoca de inmediato los terminales perdidos o de personas que dejan la empresa.
- Mantén la app actualizada.
- No compartas capturas de pantalla con datos de clientes.

## Notificar una vulnerabilidad

**No abras una incidencia pública.** Contacta de forma privada con el responsable del proyecto a través de los datos de contacto de este perfil de GitHub.
