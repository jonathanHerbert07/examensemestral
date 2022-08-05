# La instalación de openai retro, se hace atraves de python 3 utilizando pip.
Deben crear la carpeta.
Clonen el repositorio de python usando la opcion de fork en github: https://github.com/dsapandora/sonic_controller_data_capture.
1. ```git clone https://github.com/dsapandora/sonic_controller_data_capture```
dentro del sonic_controller_data_capture ejecutor lo siguiente
2. ```virtualenv -p python3 env```
3. ```source env/bin/activate```
4. ```pip3 install gym-retro```
5. Luego es necesario que importen el juego de sonic a la base de datos gym. Recuerden que el juego es ilegal distribuirlo en linea asi que no pueden subirlo en el entregable sino les banearan su repositorio.
6. Para impotar el juego creen una carpeta llamada roms y colocan ahi el archivo md con el juego luego ejecuten: ```python3 -m retro.import roms```
7. Esto indicara un mensaje de que el rom se ha importado a retro gym
8. Ahora deben ejecutar el codigo de ejemplo y probar los niveles en vectorman. Parte de su trabajo sera encontrar los niveles que deben utilizar para el entrenamiento.
9. les adjunto igualmente un ejemplo de software que se utiliza para capturar datos. Ahi esta el ejemplo de los controles. Y que significa cada posiciion del arreglo en sonic. Para ussarlo necesitaran:
numpy, cv2 y pygame para controlar el juego.

10. Los resultados se miden basado en cuanto avance la posicion x de la observacion el personaje de principal del juego, deben promediar eso para dar el resultado en una tabla.

# El entregable
1. archivos: un video en youtube como la muestra entrenamientos, un articulo de dos paginas donde se compare los resultados de la tecnica que utilizaron contra los resultados obtenidos por los participantes del concurso openai retro.
2. Una prueba el día viernes de la ejecución de su tecnica con sonic en un dominio desconocido.
3. El codigo colocado en un repositorio de github para ser revisado. Para revisar habran un pull request de su fork hacia mi reposotorio. Su repositorio debe tener una carpeta con su nombre y su codigo.
