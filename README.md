# Robot-Scara

<p align="center">
 <img width="100px" src="https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/robot.svg" align="center" alt="Robot Scara" />
 <h2 align="center">Robot Scara</h2>
 <p align="center"><b>Control de robot SCARA mediante HMI (Interfaz Hombre-Máquina) y su respectiva simulación.</b></p>

</p>
  <p align="center">
    <a href="https://github.com/cabustillo13/Robot-Scara/actions/new">
      <img alt="Tests Passing" src="https://github.com/anuraghazra/github-readme-stats/workflows/Test/badge.svg" />
    </a>
        <a href="https://github.com/cabustillo13/Robot-Scara/issues">
      <img alt="Issues" src="https://img.shields.io/github/issues/cabustillo13/Robot-Scara?color=0088ff" />
    </a>
    <a href="https://github.com/cabustillo13/Robot-Scara/pulls">
      <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/cabustillo13/Robot-Scara?color=0088ff" />
    </a>
    <br />
    <p align="center">
    <a href="https://github.com/cabustillo13/Robot-Scara/blob/master/README.md">Español</a>
    ·
    <a href="https://github.com/cabustillo13/Robot-Scara/blob/main/Traducciones/English.md">English</a>
    ·
    <a href="https://github.com/cabustillo13/Robot-Scara/blob/main/Traducciones/Portugu%C3%AAs%20Brasileiro.md">Português Brasileiro</a>
  </p>
</p>

El objetivo general del proyecto es la construcción de un sistema de realidad virtual que permita la programación de un brazo robótico industrial de forma rápida, sencilla y segura, mediante el desarrollo de una interfaz de usuario desarrollada en software y, dispositivos de Interfaz Hombre Máquina (HMI) en hardware de modo que ambas partes interactúen entre sí. La finalidad es lograr que un usuario final, sin conocimientos de programación ni de robots, logre definir fácilmente el movimiento y todas las acciones necesarias a realizar por un robot físico.

### HMI, GUI y Robot Físico

El HMI está conformado por 5 sensores MPU6050 transmitiendo datos a 3 Nodemcu, los cuales tienen asignados 3 IPs estáticas y sus respectivos puertos.

El robot físico cuenta con una GUI (Interfaz gráfica) que recibe todos los datos por socket, procesa los paquetes de datos y luego por serial envia la información al robot para que ejecute las maniobras.

La simulación corre por Coppelia Sim que está conectado por un puerto asignado al Jupyter-Lab. Este recibe por socket toda la información del HMI, consume una API de comunicación y luego envia todas las maniobras al Robot Virtual.

![Equipo](https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/equipo.png)


### Escenario 0: Calibración 

Se muestra cómo se domina el HMI con la simulación. Y que el usuario se pueda percatar de sus acciones.

![Escenario 0](https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/escenario0.png)


### Escenario 1: Circuito de Producción

Permite al usuario adentrarse en un proceso de una planta de producción y operar el robot. La idea es tomar un objeto (cilindro) de la banda transportadora en movimiento y colocarlo correctamente en la otra cinta transportadora o la mesa fija. 

![Escenario 1](https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/escenario1.png)

### Escenario 2: Evaluar motricidad fina y control del Robot

Pusimos una pared con la intención que el usuario se coloque los lentes de realidad virtual y opere a distancia el robot colocado en otra sala. El usuario debe tomar cada uno de los elementos en la parte superior de los paralelepipedos y trasladarlos hasta la mesa.

![Escenario 2](https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/escenario2.png)

# Video Demo

![Demostración](https://github.com/cabustillo13/Robot-Scara/blob/main/Recursos/videoDemo.gif)

# Autores

- Carlos Bustillo   | cabustillo13@hotmail.com
- Rodrigo Pérez     | rodrigoperez2110@gmail.com
- Diciembre 2020
