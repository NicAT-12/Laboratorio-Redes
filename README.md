# Laboratorio de Redes y Sistemas

Laboratorio virtual para practicar redes y administración de sistemas de forma concreta: configurar switches, levantar un dominio de Active Directory, automatizar tareas con PowerShell y resolver problemas con método.

Cada práctica queda documentada acá: diagrama, comandos usados, capturas y, cuando corresponde, los scripts.

## Sobre mí

Soy Nicolás, de Buenos Aires. Vengo del soporte técnico (niveles 1 y 2): gestión de tickets, resolución de incidentes, atención a usuarios y coordinación con consultores externos. Este laboratorio es mi forma de profundizar en redes y administración de sistemas con práctica real, y de dejar evidencia de lo que aprendo.

## Entorno

| Equipo | Uso |
|---|---|
| Notebook (16 GB de RAM) | Práctica de redes con Packet Tracer |
| PC principal (32 GB de RAM) | Máquinas virtuales: Windows Server, clientes, pfSense, Linux |

## Fases del laboratorio

| Fase | Tema | Estado |
|---|---|---|
| 0 | Base teórica: subnetting, OSI, TCP/IP, DNS y DHCP | En paralelo |
| 1 | Redes con Packet Tracer: VLANs, trunking, DHCP, NAT, ACLs, router on a stick, port security | En curso |
| 2 | Active Directory base: dominio, DNS, DHCP, OUs, usuarios y grupos | Pendiente |
| 3 | Administración y PowerShell: GPOs, carpetas compartidas, delegación, scripts | Pendiente |
| 4 | pfSense y segmentación de red | Pendiente |
| 5 | Linux, monitoreo y VPN: Samba o bind9, Zabbix, WireGuard | Pendiente |
| Transversal | Troubleshooting con método: informes de fallas provocadas | Se practica en todas las fases |

### Prácticas completadas

- **Fase 1 · 01 – VLANs:** creación de VLANs, asignación de puertos y verificación de aislamiento entre VLANs.
- **Fase 1 · 02 – Trunking:** dos switches unidos por un enlace trunk, con VLANs compartidas entre ambos.

## Estructura del repositorio

Una carpeta por fase, y dentro de cada práctica:

```
fase-X/
└── NN-nombre-de-la-practica/
    ├── README.md      → objetivo, topología, direccionamiento y comandos
    ├── archivo.pkt    → archivo de Packet Tracer (o scripts, según la fase)
    └── Capturas/      → evidencia de cada paso
```

## Cómo leer cada práctica

Cada README de práctica incluye:

1. **Objetivo:** qué se quiere lograr.
2. **Topología y direccionamiento:** diagrama y tabla de IPs.
3. **Comandos utilizados:** la configuración paso a paso.
4. **Verificación:** pruebas y capturas que muestran el resultado.

## Troubleshooting

En cada fase se rompe algo a propósito (gateway mal configurado, DHCP apagado, DNS que no resuelve, VLAN mal asignada, GPO que no aplica) y se resuelve siguiendo siempre el mismo orden:

1. Verificar servicios centrales (DHCP, DNS).
2. Usar `ping`, `tracert`, `nslookup`, `ipconfig` y Wireshark si hace falta.
3. Revisar qué cambió recientemente.

Cada caso se documenta como un mini informe: **síntoma, diagnóstico, causa y solución**.

## Herramientas

Cisco Packet Tracer · Windows Server · Active Directory · PowerShell · pfSense · Ubuntu Server · Zabbix · WireGuard · Wireshark

## Contacto

Email: nicotissoni12@gmail.com