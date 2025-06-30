# P3_MSR
Repositorio para la práctica 3 de la asignatura de modelado y simulación de robots


## Gráfica 1
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/posicion.png" alt="explode"></a> 
</div>
Esta gráfica muestra la evolución de la posición angular de las cuatro ruedas del robot (joint wheel_link_joint, wheel_w2_link_joint, wheel_w3_link_joint, wheel_w4_link_joint) a lo largo del tiempo.
En la fase inicial, las ruedas parten de cero y muestran un incremento brusco hasta estabilizarse, reflejando la arrancada del robot. A partir de ese momento, las posiciones permanecen constantes, lo que indica que el robot ha llegado a la zona de trabajo y se dispone a realizar la tarea de pick and place.
Los valores están normalizados entre 0 y 2𝜋 radianes, por lo que un pico alrededor de 6 rad equivale a casi una vuelta completa de la rueda.


## Gráfica 2
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/aceleracion_ruedas.png" alt="explode"></a> 
</div>
Ahora vemos la aceleración angular aproximada e las cuatro ruedas del robot, calculada como la derivada de su velocidad angular.
Se observan picos de aceleración elevados al inicio, que corresponden a las fases de arranque y los cambios de velocidad repentinos. Estos picos reflejan la respuesta dinámica rápida de los motores de las ruedas cuando reciben órdenes de movimiento a través de la teleoperacion.
Una vez superada la fase de arranque, la aceleración cae a cero y se mantiene constante, indicando que las ruedas giran a velocidad estable o permanecen en reposo (a velocidad 0) sin nuevas órdenes de aceleración, en coherencia con la tarea de pick and place posterior donde el robot permanece detenido.




## Gráfica 3
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/gasto.png" alt="explode"></a> 
</div>
En este gráfico se presenta el esfuerzo (torque o fuerza) aplicado en cada joint del robot: ruedas, articulaciones del brazo, y gripper.
Se aprecian zonas de valores muy elevados (picos tanto positivos como negativos), lo que se corresponde a maniobras exigentes como el cierre de la pinza o los movimientos del brazo.
Las ruedas también presentan picos de esfuerzo al inicio de la trayectoria, consistentes con el impulso inicial. Muchos esfuerzos caen a cero o se estabilizan, reflejando que el sistema alcanzó un estado de reposo.


## Enlace al rosbag
[rosbag](https://urjc-my.sharepoint.com/:f:/g/personal/g_alcocer_2020_alumnos_urjc_es/EgEtQe_PBxRLiI711psuAZgBubBK_cvO-F3dFsrltYoe0w?e=eZ6Wk8)


## otras fotos
### sujetando un cubo
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/hold.png" alt="explode"></a> 
</div>

### soltando un cubo
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/drop.png" alt="explode"></a> 
</div>

### parte A tfs con robotmodel
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/parteA_tfs_robotmodel.png" alt="explode"></a> 
</div>

### parte A tfs sin robotmodel
<div align="center">
<img width=600px src="https://github.com/GuilleAQ/P3_MSR/blob/main/resources/figures/parteA_tfs.png" alt="explode"></a> 
</div>
