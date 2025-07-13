# Laboratorio 1 - Compiladores 2025


## Nancy Mazariegos 22513



## Pasos para la ejecución

### 1. Moverse a la carpeta del proyecto
```bash
cd /Users/nancymazariegos/Documents/Repos/lab-1-compis
```

### 2. Construir imagen y correr el contenedor
```bash
docker build --rm -t lab1-image . && docker run --rm -ti -v "$(pwd)/program":/program lab1-image
```

### 3. Generar archivos con ANTLR
Ya dentro del contenedor:
```bash
antlr -Dlanguage=Python3 MiniLang.g4
```

### 4. Ejecutar el analizador sintáctico
```bash
python3 Driver.py program_test.txt
```



## Link a video

https://youtu.be/9C0Lu4XQLGM


