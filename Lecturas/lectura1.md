# Crítica: *Collaborative filtering recommender systems*

*Collaborative filtering* se conoce como el proceso en que se realizan evaluaciones o recomendaciones de items a partir de la opinión o experiencia de otros usuarios. El paper detalla los tipos de algoritmos de *CF*, en donde entre ellos se encuentran:

* *Non-probabilistic Algorithms*: Estos algoritmos no están basados en una probabilidad de que a un usuario le guste un item, sino que buscan encontrar un factor que permita representar la similitud que tengan dos usuarios (o items) y, a partir de esta similitud, predecir el ranking de un item en particular basado en la opinión de los usuarios que más se parezcan en sus gustos.

* *Probabilistic Algorithms*: A partir de herramientas de probabilidad y estadística, buscan predecir valorizaciones para distintos items. Por ejemplo, a través de un árbol de decisiones se va recorriendo los nodos y para cada uno de los nodos si cumple con la condición, se traduce en una probabilidad y al llegar al último nodo se calcula la probabilidad a través de todos los nodos que recorrió el usuario.

Por otro lado, se habla sobre los tipos de rating que tiene un sistema, por ejemplo, existen los ratings implícitos y los explícitos, la diferencia es que para los primeros el usuario no necesita ingresar su calificación directamente al sistema, sino que es este último el que la debe recopilar y procesar, mientras que para los segundos el rating es el usuario el que lo debe ingresar personalmente. También hay otras categorías como la escala en que se encuentra un Rating: unario, binario o entero. 


El paper solamente dio una descripción el trabajo ya existente en el área de *Collaborative filtering*, por lo tanto, no debería haber muchas cosas que criticar de manera negativa sobre este. En general me interesó mucho los tipos de algoritmos que existían y la recolección de ratings implícitos. Un caso cercano que se me vino a la mente fue el de Netflix en donde en un principio se partió con ratings explícitos, en el que había que calificar con estrellas las películas, pero con el tiempo se fueron eliminando estos ratingis y solamente se quedaron los ratings implícitos, en donde el sistema es el que recolecta estos datos a partir de la experiencia de los usuarios, de esta forma genera un perfil personalizado para cada persona. 

En otro tema, se me ocurre que se podría utilizar Deep Learning para poder abstraer la relación entre usuarios e items, de esta forma la red recibiría como *input* un tensor con los rankings que un usuario le ha dado a otros items y tendría como *output* un rating para un item específico. De esta forma, en el caso de Netflix la red también podría utilizar otras categorías como el tipo de película, duración o idioma en el que está grabada, de esta forma se puede personalizar aún más las recomendaciones.


