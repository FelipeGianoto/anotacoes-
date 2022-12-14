- <b>Funções anônimas (sem nome)</b>
- <b>Mais limpa, podendo ser feita em 1 linha</b>

 <h5>Exemplo</h5>
List<Funcionario> funcionario = new ArrayList<Funcionario>()

List<Funcionario> funcionariosQuePagam= new ArrayList<>()

- Filtrar por funcionários com salário maior que 1903 E adicionar na lista funcionariosQuePagam;

funcionarios.forEach(f) -> { 
             If(f.getSalario() > 1903.9){ funcionarioQuePagam.add(f);
    });
funcionariosQuePagam.forEach((f) -> sysout(f.getNome()));



 <h5>Stream API do java 8 </h5>
-Trouxe o objeto stream que a partir dele podemos chamar métodos como:
-Stream-> ajuda a manipular listas de uma maneira fácil os loops como forEach ficam por conta da API, assim pode-se preocupar apenas com regras de negócios
-Filter ->filtra por uma determinada condiçao 
-Map -> vai pegar os dados q filtrou e vai trazer um dos atributos desse dado.
-Collect -> monta a lista trazendo essa coleção 

  <h5>Exemplo</h5>
- Filtrar por funcionários com salário maior que 1903 E retornar os NOMES;

List<Funcionario> funcionario = new ArrayList<Funcionario>();

List<String> funcionarioQuePagamIr = funcionarios.stream();
               .filter(f -> f.getSalario() > 1903.98) 
               .map(f ->f.getNome())
               .collect(Collectors.toList())

funcionarioQuePagamIr.forEach((f) -> sysout(f)); 





- Java Stream Api: manipulando coleções de forma eficiente 







- As operações podem ser encadeadas umas após a outras(pipeline), de forma q uma operação seja a entrada da outra 
- Passo a passo do processamento de uma Stream

1 - Stream é obtida de alguma fonte de dados(coleçao, array ou I/O)
2 - filter() retorna uma nova Stream com elementos filtrados
3 - A Stream anterior é ordenada com a operação sorted()
4 - Agora, a Stream da operação sorted() é mapeada com a operação map()
5- Por fim, a operação collect(), uma operação de redução, é aplicada para obter o resultado final em algum tipo de objeto diferente de Stream


- Filter()
List<Order> order= new ArrayList<Order>();
Stream<Order> bigOrders = order.stream()
                                               .filter((order) -> order.getTotal() > 999.00);

- Sorted()
List<Order> order= new ArrayList<Order>();
Stream<Order> sortedOrder = order.stream()
                             .sorted((order1, order2) -> Double.compare( 
                                               order1.getValue(), order2.getValue()));

- Map()
List<Order> order= new ArrayList<Order>();
Stream<Order> sortedOrder = order.stream()
                                     .map((order) -> order.getValue());




