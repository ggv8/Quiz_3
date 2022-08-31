# Respuestas

a) donde itr es un iterador y lst es una lista dinámica
while( itr != lst.end( ) )

R/ Se tiene una estructura de control cuya condición compara dos iteradores; el método end() de la lista retorna un puntero Node bajo la abstracción de un iterador y sus operaciones asociadas. Este puntero retornado es el miembro "previous" del nodo sentinela "last", propio de la lista. De manera que while repetirá un proceso si el nodo apuntado por 'itr' no sea el último nodo de la lista 'lst'.

b) donde StringNode es una clase que existe
StringNode* next;

R/ Es la declaración de un miembro de la clase StringNode bajo el identificador 'next'. Dicho miembro es un puntero a otras instancias de tipo StringNode. (Nota: Se asume que esta declaración ocurre dentro del contexto de la clase en base a su nombre)

c) void addFront(const string& e)

R/ Se declara un método "addFront" que recibe una referencia de tipo string declarada constante. En tal caso, este proceso no podrá realizar ninguna operación que modifique los contenidos del parámetro. Además, dado el nombre del método, se puede esperar que la función que cumple es agregar el valor recibido a un Nodo, para luego insertarlo en la primera posición de una lista.

d) donde SLinkedList es una clase que existe
template <typename E>
class SLinkedList {
}

R/ La declaración de la clase SLinkedList es precedida por la declaración de un template para un tipo nombrado "E". Debido a ello, SLinkedList puede declarar sus miembros bajo un tipo genérico E. Por ejemplo, en lugar de contener nodos dedicados a un tipo particular de dato (como StringNode), puede utilizar otras estructuras genéricas como Node<E>.
