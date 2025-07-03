# Repositorio de Lab04

Este es el repositorio para el **Lab04** de [Curso/Tema]. En este repositorio se guardan los archivos correspondientes a las actividades y ejercicios realizados durante el lab.

## Pasos para crear y subir el repositorio a GitHub

### 1. Crear el repositorio localmente
1. Se creó una nueva carpeta llamada `lab04` en el escritorio de la computadora.
2. Iniciamos el repositorio con el comando:

   ```bash
   git init
📄 Archivos creados
.gitignore

main.py

requirements.txt

Otros archivos como lab_part1.txt, config.txt, etc.

📥 Commit inicial
Se realizó el commit inicial con los archivos base:

bash
Copiar
Editar
git add .
git commit -m "feat: initialize Python project"
Luego se enlazó con GitHub:

bash
Copiar
Editar
git remote add origin https://github.com/promandaAOHT/lab04.git
git branch -M main
git push -u origin main
➕ Commits adicionales (Lab anterior)
Se agregaron 3 commits con partes del laboratorio anterior, por ejemplo:

bash
Copiar
Editar
git commit -m "docs: agregar parte 1 del laboratorio anterior"
git commit -m "docs: agregar parte 2 del laboratorio anterior"
git commit -m "docs: agregar parte 3 del laboratorio anterior"
🧪 Simulación de error
Se introdujo un error de sintaxis en main.py:

python
Copiar
Editar
def saludar()
    print("Hola")
Se ejecutó el archivo y arrojó un SyntaxError.  
py main.py
♻️ Revertir el commit con error
El commit con el error se hizo así:

git commit -m "feat: agregar función saludar con error"
Y se eliminó el último commit con:

git reset --hard HEAD~1
🗑️ Borrar commits en Git
Con línea de comandos
Borrar el último commit pero mantener los cambios:

git reset --soft HEAD~1
Borrar el commit y también los cambios:

git reset --hard HEAD~1
Revertir un commit específico (sin borrar historial):

git revert <commit_id>