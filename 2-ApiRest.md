<h1> Api </h1>

De uma forma simples O conceito de API nada mais é do que uma forma de comunicação entre sistemas. 
Ou seja, elas permitem a integração entre dois sistemas, em que um deles fornece informações e serviços que podem 
ser utilizados pelo outro, por exemplo um sistema de meteorologia e o outro sistema utiliza desses dados por meio da API.

<h1> Rest </h1>

<b>Representational State Transfer</b>, abreviado como REST, não é uma tecnologia, uma biblioteca, e nem tampouco uma arquitetura,
mas sim um modelo a ser utilizado para se projetar arquiteturas de software distribuído, baseadas em comunicação via rede.


Uma das principais vantagens da API Rest é a separação de aplicações front-end e back-end, que é 
considerada um passo fundamental para a proteção do armazenamento de dados. Assim, são realizadas apenas as trocas de informações, 
e não há tratamento de regras de negócio


<h1> Utilização do Spring boot na criação da API - integração com java </h1>

Projeto Exemplo: 

Você está trabalhando no desenvolvimento de uma API Rest para uma aplicação de um e-commerce, 
utilizando o Spring Boot, e cria uma classe Controller da seguinte maneira:

    @RestController
    @RequestMapping("/produtos")
    public class ProdutoController {

        @GetMapping
        public String produtosEmEstoque() {
            return "Produtos em estoque...";
        }
    }

para que o Controller esteja mapeado corretamente nao se utiliza a anotação @Controller e sim @RestController

 Quando desenvolvemos APIs e queremos que todos os seus recursos fiquem disponíveis a qualquer cliente HTTP, 
 uma das coisas que vem à nossa cabeça é o CORS (Cross-Origin Resource Sharing), em português, “compartilhamento de recursos com origens diferentes”. 
 consumir e disponibilizar APIs
 
 <h1> CORS </h1>
 
O CORS é um mecanismo utilizado para adicionar cabeçalhos HTTP que informam aos navegadores para permitir que uma aplicação Web seja executada em uma origem e acesse recursos de outra origem diferente. 
Esse tipo de ação é chamada de requisição cross-origin HTTP. Na prática, então, ele informa aos navegadores se um determinado recurso pode ou não ser acessado.

Para configurar o CORS e habilitar uma origem específica para consumir a API, basta criar uma classe de configuração como a seguinte:

@Configuration
public class CorsConfiguration implements WebMvcConfigurer {

    @Override
    public void addCorsMappings(CorsRegistry registry) {
        registry.addMapping("/**")
            .allowedOrigins("http://localhost:3000")
            .allowedMethods("GET", "POST", "PUT", "DELETE", "OPTIONS", "HEAD", "TRACE", "CONNECT");
    }
}


