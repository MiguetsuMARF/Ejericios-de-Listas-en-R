### 1 ###

# Crea una lista que contenga al menos cuatro tipos diferentes de datos 
# (incluyendo al menos un vector, una matriz, y un data frame). 
# Luego, escribe código para acceder a cada uno de estos elementos por su índice.

Mi_primer_lista <- list (
  Nombres = c("Santiago", "Miguel", "Ivan"),
  Horas_de_trabajo = 17,
  Numero_de_cafes = matrix(c(1, 2, 3, 4), nrow = 2),
  Tipos_de_cabello = data.frame(
    color = c("rojo", "azul", "negro", "castaño"),
    longitud = c("largo", "corto", "corto", "pelon"),
    tipo = c("quebrado", "liso", "chino", "pelon")
  )
)

Mi_primer_lista

# Hay dos formas de acceder, con el indice o con el nombre.
# si queremos acceder a los tipos de cabello:

Tipos_cabello <- Mi_primer_lista[[4]]
Tipos_cabello

# Si queremos acceder a los numeros de cafes:

num_cafes <- Mi_primer_lista$Numero_de_cafes
num_cafes

### 2 ### 

# Añade un nuevo elemento a la compleja_lista que sea otra lista conteniendo 
# información relevante a un experimento microbiológico (p.ej., fechas, resultados 
# de crecimiento, tipo de medio de cultivo). Accede a un elemento específico dentro 
# de esta lista anidada.

Mi_primer_lista_expandida <- list(
  Mi_primer_lista[[1]],
  Mi_primer_lista[[2]],
  Mi_primer_lista[[3]],
  list (
    Bacterias = c("E.coli", "Salmonella", "Pseudomonas", "Borrelia", "Babesia"),
    Medio_cultivo = c("Agar Sangre", "PDA", "Agar Agar", "Mc Conkey"),
    Matriz_de_Crecimiento = matrix ((rnorm(6)), nrow = 3)
  ),
  Mi_primer_lista[[4]]
)

# Para sacar de la lista anidada debemos utilizar doble doble corchete.

Mi_primer_lista_expandida[[4]][[2]] -> Medios
Medios

### 3 ###
# Almacena datos de producción en experimentos de fermentación.

Fermentacion <- function (bacteria, tasa_fermentacion, tasa_consumo){
  consumo_inicial <- glucosa
  while (co2 < 48.9){
  co2 <- co2 + tasa_fermentacion
  glucosa <- glucosa-tasa_consumo
  tiempo <- tiempo + 1
  }
  print(paste(bacteria, co2, consumo_inicial - glucosa, tiempo)) 
}

datos <- data.frame(
  Bacterias = c("Lactobacilus", "Bifidobacterium", "E.coli"),
  tasa_fermentacion = as.numeric (c(0.489, 0.567, 0.1245)),
  tasa_consumo = as.numeric (c(0.87, 0.96, 0.12))
)
str(datos)
glucosa <- as.numeric(100)
co2 <- as.numeric(28.9)
Fermentacion(datos[1,1], datos[2,1], datos[3,1])

# Suponiendo entonces 

## Crea una lista fermentacion con 4 elementos, cada uno representando 
## un experimento de fermentación.


## Cada elemento debe ser una lista con: Cepa, Condición, ProducciónEtanol.
## Encuentra la condición con la mayor producción de etanol.