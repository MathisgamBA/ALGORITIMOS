1-Estruturas de dados referem-se à organização, gestão e armazenamento de dados para facilitar o acesso eficiente e manipulação. Elas estabelecem formatos e regras que definem a organização dos dados.

2-Essenciais para otimizar tempo de execução e uso de memória em operações comuns, como inserção, busca, remoção e atualização de dados. Além disso, organizam os dados de maneira significativa para a aplicação.

3-Array:

 Armazena uma coleção de elementos do mesmo tipo sob um único nome.
Quando utilizar: Para acesso rápido por índice, tamanho conhecido antecipadamente e ordem relevante.
Array Estático: É definida a quantidade máxima de registros permitidos na criação do array.
Exemplo:


public class Exemplo {
    int valores[] = new int[6]; // array com capacidade máxima de 6 registros
}
Array Dinâmico: A capacidade máxima pode variar, com a utilização de métodos.
Exemplo:

public class Exemplo {
    int valores[]; 
    public Exemplo(){
        this.valores = new int[6];
    }
}
Lista:

 Define uma lista ordenada de elementos com índices associados, permitindo com que possamos selecionar um registro em alguma posição dentro da lista.
Quando utilizar: Para coleção ordenada, adição/remoção frequentes e ordem relevante.

ArrayList:   Um ArrayList, da interface List, implementa um vetor dinâmico, que pode diminuir ou crescer de forma dinâmica.

Exemplo:
public class Exemplo {
    public static void main(String[] args) {
        List<String> frutas = new ArrayList<>();
        frutas.add("Maçã");
        frutas.add("Banana");
        System.out.println(frutas.get(1)); // Selecionando uma fruta com base no seu índice
        System.out.println("Frutas: " + frutas);
    }
}

Fila:

 É uma estrutura de dados que segue o princípio "primeiro a entrar, primeiro a sair" sem duplicatas.
Quando utilizar: Processamento em ordem de entrada, agendamento de tarefas e controle de recursos compartilhados.
Exemplo:

public class Exemplo {
    public static void main(String[] args) {
        Queue<String> tarefas = new LinkedList<>();
        tarefas.add("Estudar");
        tarefas.add("Trabalhar");
        tarefas.add("Descansar");
        System.out.println("Primeira fila: " + tarefas);
        String removida = tarefas.remove();
        System.out.println(removida); // O primeiro elemento que foi adicionado é removido
        System.out.println("Nova fila: " + tarefas);
    }
}

Pilha:

 A pilha (stack) segue o princípio "último a entrar, primeiro a sair", usado para desfazer ações e rastreamento de chamadas de função.                                                                                                                               
Quando utilizar: Quando é necessário o processamento de itens em ordem reversa, rastrear chamadas de funções de programa e desfazer ações em um aplicativo  
                                                                                                                                                                    Exemplo:
public class Exemplo {
    public static void main(String[] args) {
        Stack<String> operacoes = new Stack<>();
        operacoes.push("Adição");
        operacoes.push("Subtração");
        operacoes.push("Multiplicação");
        System.out.println("Topo da pilha: " + operacoes.peek());
        String removida = operacoes.pop();
        System.out.println("Operação removida: " + removida); // O último elemento a ser adicionado foi removido
        System.out.println("Nova pilha: " + operacoes);
    }
}
