---
title: "Lab 01 - Instalación de Metasploitable 3"
date: 2026-05-24 15:56:00
categories: [lab,setup]
tags: [metasploitable, virtualbox, kali]
---
## Creación de la VM Metaploitable 3
[Metaploitable es una plataforma que se usa para pruebas de seguridad. Contiene diversas vulnerabilidades que se pueden explotar. En el lab servirán para realizar nuestras pruebas.]
[Un archivo .OVA es una máquina virtual completa empaquetada mientras que un archivo .ISO es una imagen de disco]

![Creación de la VM en VirtualBox](images/captura1.png)

![ISO montado en la VM](images/captura2.png)

## Configuración de red

[Se usa NatNetwork para que las máquinas virtuales tengan acceso a Internet y, al mismo tiempo, puedan comunicarse entre ellas dentro de una red virtual privada.]

![Configuración de red](images/captura3.png)
 
 ## Verificación de conectividad

  | Máquina | IP asignada |
  |:--------|:------------|
  | Kali Linux (atacante) | 10.0.2.X |
  | Metasploitable 3 (victima) | 10.0.2.Y |

  ![Resultado nmap](images/captura4.png)
  ![Ping exitoso](images/captura5.png)