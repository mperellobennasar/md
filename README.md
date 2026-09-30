# Titulos
MarkDown permite añadir titulos de varios tamaños, indicados por 1 o varios **#**, de la siguiente manera:

# Titulo 1
## Titulo 2
### Titulo 3
### ...
###### Titulo 6


# Texto
Se permite dar formato a un texto usando diferentes etiquetas:

*Italic con \* o \_ antes y despues del texto*

**Bold con \*\* o \_\_ antes y despues del texto**

Se pueden combinar ambos ***italic y bold***

~~Subrallado~~ con \~\~ antes y despues del texto

`Inline code con ` \` ` antes y despues del texto`


# Listas
Existen los siguientes tipos de listas:

- No numeradas
  - a
  - b
  - c

0. Numeradas
    1. a
    2. b
    3. c

- Tareas

- [x] a
- [ ] b
- [ ] c

# Elnaces e imagenes

Se puede añadir un enlace:

[Bases de MarkDown](https://www.markdownguide.org/basic-syntax/)

O una imagen:

![print hello world](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRc_d9hBSAhw5UGoIGCKhm3KWnX6wGLGQdv6PQJmiXneg&s)

# Codigo

Se puede introducir un bloque de codigo con \~\~\~ antes y despues del texto:

*Se puede indicar el lenguaje para resaltar despues del \~\~\~*

*En este caso* **asm**:

~~~asm
global _start
  section   .text

_start: 
  mov rax, 1                        
  mov rdi, 1                         
  mov rsi, message                      
  mov rdx, 13
  syscall
  mov rax, 60
  xor rdi, rdi
  syscall
          
section .data
  message: db "Hello, World", 10
~~~

# Tablas

MarkDown tambien permite añadir tablas usando \- y \| para indicar los bordes de cada celda: 


| Columna A | Columna B    | Columna C | 
| --------- | ---------    | --------- |
| Contenido | *formateado* | `Codigo`  |
|           | Contenido    | ~~Linea~~ |
| Vacio ^   | Text         | Contenido |

# Citas y decoradores

Se pueden citar contenidos con el caracter **\>**:

> An idiot admires complexity, a genius admires simplicity, a physicist tries to make it simple, for an idiot anything the more complicated it is the better
>
>
> -Terry A. Davis
> 
>
> >Tambien se pueden anidar varias citas con el mismo caracter
> >
> >Asi como añadir cualquier etiqueta, como texto **con** *formato* `o codigo`

Para estructurar un documento, puede ser util usar un separador horizontal introduciendo "---":

---


Al posicionar esta linea justo despues de un texto, se va a crear un titulo automaticamente:

Test
---
