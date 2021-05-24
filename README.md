# PROXMOX Virtual Environment

![](images/proxmox.png)

PROXMOX VE “Virtual Environment” es un entorno de virtualización de servidores de código abierto. 
Está en distribuciones GNU/Linux basadas en Debian con una versión modificada del Kernel RHEL (Red Hat Enterprise Linux) y permite el despliegue y la gestión de máquinas virtuales y contenedores. Proxmox VE incluye una consola Web y herramientas de línea de comandos, y proporciona una API REST para herramientas de terceros. Dos tipos de virtualización son compatibles: los contenedores basados con LXC (Linux Containers) y la virtualización con KVM (Kernel-based Virtual Machine). Viene con un instalador e incluye un sitio Web basado en la interfaz de administración.

## Característias principales: 

- **Administrador Web GUI** se basa en el marco de JavaScript ExtJS y puede usarla con cualquier navegador moderno, para configurar los servidores físicos, clusters, máquinas virtuales, respaldos y restauracion, snapshots. No es necesario instalar aplicaciones de terceros.

- **Virtualización para la mayoría de Sistemas Operativos**, en versiones de 32 y 64bits. Linux en todas sus distribuciones, Microsoft desde windows 98 hasta windows 10 y windows server desde 2000 hasta 2019, Solaris, AIX, entre muchos más compatibles con KVM.

- **Máquina virtual basada en kernel** (KVM) es una solución para implementar virtualización sobre Linux.  Puede funcionar en hardware x86/x86_64 y es necesario que el microprocesador tenga soporte de virtualización ya sea Intel VT-x o AMD-V.

- **Virtualización basada en contenedores** (LXC), es una alternativa para ejecutar máquina Linux en espacios separados. A diferencia de la virtualización KVM este funciona como un módulo agregado al servidor físico y hace uso directo del hardware.

- **Los Respaldos** se administran a través de su interfaz Web. Puede efectuar un respaldo de forma inmediata o programado. La restauración es simple, solo debe de seleccionar el backup a restaurar y listo.

- **Las Instantánea en vivo** le permite hacer copias de máquinas Virtuales incluyendo el contenido de la RAM, su configuración y el estado de los discos virtuales. Usted puede retroceder en tiempo la Maquina Virtual restaurando spanshot's.

- **Firewall** es completamente personalizable y permite configuraciones complejas a través de la conosla web o linea de comandos.

- **Alta Disponibilidad** con al menos 3 nodos o equipos con proxmox en cluster, si alguno de los nodos falla, las maquinas virtuales migran en automatico hacia los otros nodos.

- **Migración en vivo y en linea** le permite mover las maquinas virtuales entre nodos sin ningún tiempo de inactividad o efecto perceptible por parte del usuario final, con los recursos en almacenamiento compartido no hay necesidad de mover los discos virtuales.

- **Integración con NAS o SAN** ya sea a través de Fibra Canal, iSCSI Over Ethernet o NFS.

- **Almacenamiento Hiperconvergente** con Ceph o ZFS de facil administración utilizando solo la interfaz web.
