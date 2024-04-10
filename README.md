# Practica Ansible 
En este repositorio se explicaran los pasos para ejecutar un Contenedor Con Super Mario Infinite 
## Tecnologias
1. Terraform
2. Azure 
3. Ansible

## Primer Paso
Tener la infraestructura para una Maquina Virtual, y montarla en Azure

## Segundo Paso
Asegurarse e configurar el acceso ssh del repo de este repo, para que la IP publica sea la misma de la maquina virtual y los credenciales

## Tercer Paso
Ejecutar los Siguientes Comandos
```bash
ansible-playbook -i inventory/hosts.ini playbooks/install_docker.yml
ansible-playbook -i inventory/hosts.ini playbooks/run_container.yml
sudo chmod 755 .
```
## Cuarto Paso
Ingresamos en azure a los network settings, y agregamos una regla de ingreso de puerto
<img width="585" alt="Captura de pantalla 2024-04-09 a las 22 10 05" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/0c52df6f-556d-4028-85fb-f9acfdc68a5d">

# Evidencia de funcionamiento
<img width="1152" alt="Captura de pantalla 2024-04-09 a las 22 31 27" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/fcf3593a-41b7-4578-9d25-3631abe36dc5">
<img width="1149" alt="Captura de pantalla 2024-04-09 a las 22 30 18" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/6f91f114-612d-458f-8787-f4c02abb5428">
<img width="1463" alt="Captura de pantalla 2024-04-09 a las 22 11 19" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/47aab6df-05ed-4a38-bfb2-e665e59ff1ed">
<img width="1154" alt="Captura de pantalla 2024-04-09 a las 22 11 42" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/004bddb8-c4f9-403f-97fa-f83ff620513e">
<img width="654" alt="Captura de pantalla 2024-04-09 a las 22 20 17" src="https://github.com/Samuelguerrero1184/ansible-az-vm/assets/61643297/a18af41d-51ee-4f32-b5f3-bd34b06b0477">
