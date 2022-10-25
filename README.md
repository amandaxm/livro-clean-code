# Repasse Livro Clean Code 
## Vouncher de Reconhecimento Framework🚀💜

### Como distinguir um código bom 👍  de um ruim 👎

O código ruim é um código confuso que, diretamente proporcional, conforme a confusão aumenta, a produtividade da equipe diminiui, assintoticamente aproximando de zero. O livro cita as definições de um código limpo por alguns programadores conhecidos e com muita experiência, em resumo as definições foram: 

#### Um código limpo é:

- elegante, eficiente, que tem uma lógica direta
- inteligível, simples, sem duplicações
- é um código com funções limpas, nomes limpos, classes limpas  
- que foi cuidado por alguém, alguém que manteve o código simples e organizado 
- é um código com testes, mesmo que o código seja, elegante, acessível, direto e simples, se ele não tiver testes, ele não é um código limpo

### A regra do escoteiro
Um código limpo precisa ser mantido limpo, pois ele se  degrada e estraga com o tempo, dito isso, uma organização de jovens escoteiros dos EUA tem uma regra simples, que nós devemos aplicar a nossa profissão:
##### "Deixe a área do acampamento mais limpa do que como você a encontrou"💭🤺
dessa forma o código não degradaria, com mudanças simples, como nome de variáveis, reorganizando um if aninhado, eliminando um pouco da repetição,  o código se manteria limpo, ou aos poucos é possível tornar um código ruim em um código limpo.



### Como escrever códigos bons e como transformar um ruim  😢 em um bom  😀 

- Sempre escrever nomes bons e intuitivos, mesmo que grandes, mas que representam de fato o que a variável é. 
- Evitar ifs aninhados
- escrever  funções pequenas
- funções devem ter apenas um propósito. 

#### Para transformar um código ruim em um bom, basta refatorar, fazer disso um hábito, aplicando essa filosofia, aos poucos um código que antes considerado ruim, pode se tornar um código bom ✨ 


### Como criar bons nomes, boas funções, bons objetos e boas classes😎

para encontrar bons nomes demandam muito tempo, mas economizamos mais e devemos trocar quando encontrarmos nomes melhores
nome deve responder a essas questões: #### porque existe? O que faz? Como é usado?
 - Usar nomes que revelam seu Propósito
 - Se um nome precisa de um comentário então ele não revela seu propósito evitar informações erradas
 - Exemplo não referir account List a menos que realmente seja uma List, por ser algo específico para programadores. Devemos ter cuidado com nomes muitos parecidos
 - Evitar usar a1,a2 .. an, pois não oferecem informação alguma
 - Usar nomes pronunciáveis
 - Usar nomes passíveis de busca
 - Nomes de uma letra só ou números são difíceis de localizar ao longo do código.

>#### Codificar nomes simplesmente adiciona uma tarefa extra de decodificação, contratar um novo funcionário para aprender outra “linguagem” codificadora além da atual usada no código terá uma sobrecarga mental desnecessária.🤔
prefixos

ℹ Evitar utilizar prefixo, as pessoas rapidamente começam a ignorar o prefixo ou sufixo para visualizar as partes significativas do nome

#### Nomes de classes

- Devem ter nomes com substantivos, como Conta, Cliente, Produto

#### Nomes de métodos
- devem ter verbos como Excluir Página, Salvar

>Não devemos ficar com medo de mudar nomes, uma vez que for para melhor, deve ser feito🆘

#### Funções

- devem ser pequenas, no máximo 25 linhas
- blocos dentro de instruções de if, else, while, devem ter apenas uma linha, possivelmente uma chamada de outra função
- Faça apenas uma coisa

fazer apenas uma coisa por exemplo alterar um dado no banco. uma função não deve fazer mais de uma coisa🆘.

>>Não é uma boa prática na programação de acordo com o livro Clean code, uma função deve fazer apenas uma coisa. Se é para consultar um dados no banco, vai consultar o dado, se é para excluir um dado no banco, ela deve apenas excluir o dado e se é para editar um dado no banco, deve apenas editar o dado.

 - Ler o código de cima para baixo

Regra decrescente que um código de uma função, a escrita deve ser igual parágrafo você vai ler de forma corrente. Facilita o entendimento do código.

#### As funções devem ser pequenas e os blocos bem identados, que faça apenas uma coisa, o código é de cima para baixo e a função deve ter no máximo três parâmetros de entrada, assim ele descreve uma função ideal.

### Objetos

#### Lei de Deméter

O método f de uma classe C deve apenas chamar os métodos destes:

- C
- Um objeto criado por f
- Um objeto passado como um argumento para f
- Um objeto mantido em uma variável de instância de C
- O método não deve invocar métodos em objetos que são retornados por qualquer uma das funções permitidas. Em outras palavras, converse com amigos, e não com estranhos.

#### Objetos de transferência de dados

 DTOs são estruturas muito úteis, especialmente quando se comunicam com bancos de dados.

#### Conclusão objetos

>Eles expõem o comportamento e ocultam os dados. Isso facilita a adição de novos tipos de objetos sem alterar os comportamentos existentes, mas também torna difícil adicionar novos comportamentos a objetos existentes.

#### Classes 

Organização das classes 

#### Deve começar com uma lista de variáveis, as publicas, estáticas e constantes devem vir primeiro e depois as variáveis estáticas privadas
As funções públicas devem vir após as listas de variáveis 
Tarefas privadas chamadas por uma função pública, devem ser descritas logo após a pública, seguindo a regra de cima para baixo, o programa deve ser lido como um jornal
Encapsulamento

      - Ideal seria que todas variáveis e funções fossem privadas, mas não devemos ser tão radicais.
      - As vezes precisamos proteger uma variável ou função de suporte para ser acessada por um teste
      - o teste deve ter prioridade
      - primeiro devemos procurar uma maneira de manter a privacidade, perder o encapsulamento é sempre o último recurso.

 - As classes devem ser pequenas 

- Classes devem ter poucas responsabilidades, mensuramos o tamanho da classe por responsabilidade
uma classe com 5 métodos pode ter muitas responsabilidade
- O princípio de responsabilidade única

- Uma classe ou módulo deve ter apenas um motivo para mudar
- Ajuda na organização e clareza
- Devemos dividir as classes muito cheias em outras com responsabilidades únicas
- Um sistema com classes maiores, nos atrasa pois percorremos diversas coisas que não precisamos saber no momento
sistema ideal com muitas classes pequenas e não poucas classes grandes

#### Coesão

- Quão relacionadas ou focadas estão as responsabilidades da classe
- A coesão faz com que os métodos e as variáveis sejam co-dependentes, como um todo lógico
- Se uma classe perde a coesão, devemos dividí-la
  #### Objetivo => Classes devem ser coesas, organizadas e desacopladas.🎯
  
### Como formatar o código para ter uma legibilidade máxima🔍

#### Formatação

>É necessário reparar na organização, o código não deve ser emaranhado.😵
A formatação serve como  uma comunicação e essa é a primeira regra nos negócios de um desenvolvedor profissional, deve ser organizado.

#### Formatação vertical

O tamanho do arquivo não deve ser muito grande, Junit, FitNesse and Money são compostos por arquivos pequenos, nenhum ultrapassa 500 linhas e a maioria dos arquivos tem menos de 200 linhas, e alguns com milhares de linhas como Tomcat. 

Não da para definir uma regra fixa, mas, arquivos pequenos costumam ser mais fáceis de se entender que os grandes.

#### Declaração de variáveis

- deve-se declarar as variáveis o mais próximo possível de onde serão usadas.
- se a função for pequena, as variáveis podem ser declaradas no topo de cada função

#### Ordenação vertical

 - Chamadas das dependências das funções devem apontar para baixo, a função a ser chamada deve ficar embaixo da que chama
a fim de criar um fluxo natural, de um nível maior para menor

#### Formatação Horizontal

A largura de uma linha pode ser até 80, programadores preferem linhas curtas de acordo com estudo

#### Regras de equipe

>A equipe deve escolher um único estilo de formatação e todos devem usá-lo, para o software ter um estilo consistente
Assim o código terá uma boa organização
#### Um código bem formatado é mais fácil de ler e entender.🙂😉

### Como implementar completamente o tratamento de erro sem obscurecer a lógica❓
#### Usar exceções em vez de retornar códigos

- É melhor lançar uma exceção quando um erro for encontrado, dessa forma o código de chamada fica mais limpo e sua lógica não fica ofuscada pelo tratamento de erro
Fornecer exceções com contexto

#### Cada exceção deve fornecer contexto necessário para a localização de um erro
- Mencionar a operação que falhou e o tipo de falha

#### Não retornar null

- Ao retornar null estamos criando mais trabalho para nós mesmos 
- Ao invés de retornar null em um método, devemos lançar uma exceção

#### Não passar null

- Passar null para um método é pior que retornar null😣
- Podemos receber uma nullPointerException☹
- É sinal de problema e pode causar mais erros 🆘
#### O tratamento de erro é extremamente importante para a manutenção do nosso código⚠
### Como aplicar testes de unidade e praticar o desenvolvimento dirigido a testes
** Ideal: Deveríamos criar testes que garantisse que cada canto do código funcionasse como esperamos.
As três leis do TDD
1. Não se deve escrever o código de produção até criar um teste de unidade de falhas.
2. Não se deve escrever mais de um teste de unidade do que o necessário para falhar.
3. Não se deve escrever mais códigos de produção do que o necessário para aplicar o teste de falha atual.

### Como manter os testes limpos
- Testes  mal feitos é pior que não ter nenhum teste
- Quanto pior o teste, mais difícil de refatorar
- Quanto mais confuso o teste, maiores as chances de levar mais tempo escrevendo novos testes
Conforme o código de produção é modificado, os testes antigos começam a falhar e a bagunça nos testes dificulta fazê-los funcionar novamente.
a manutenção dos testes pode contribuir negativamente para a finalização do projeto. E no final podemos ser forçados a descartar todos os testes.

- Sem os testes não podemos garantir que, após as alterações no código, ele funcionasse como o esperado e que mudanças em uma parte do sistema não afetam outras partes.
Os bugs crescem🚫, e o medo de alterar o código fica maior.
- Conclusão ficamos sem testes, com um código de produção confuso e cheio de bugs.
os código de testes são tão importantes quanto o código de produção.
- Ele não é secundário, ele requer raciocínio, planejamento e cuidado.
- É Preciso mantê-lo limpo como código de produção.
os testes de unidade mantêm o códigos flexível, reutilizável e passível de manutenção. Com testes não vamos ter medo de alterar o código
- Quanto maior a cobertura dos testes↗, devemos ter menos  medo.↘

Portanto,  testes de unidade automatizados que cubram o código de produção é o segredo para manter o projeto e arquitetura o mais limpos possíveis.✔

Se não, se os testes forem ruins,  a capacidade de modificar o código fica comprometida e perde a capacidade de alterá-lo. No fim, perdemos os testes e o código se degrada.❌
### Testes limpos
Três coisas tornam um teste limpo: Legibilidade✅, legibilidade✅ e legibilidade✅. 
** Clareza, simplicidade, consistência e expressão tornam um teste legível.
### Uma afirmação por teste
Há uma escola de pensamento que diz que cada teste em JUnit deve ter uma e apenas uma instrução de afirmação (assert). Os testes chegam a uma única conclusão que é fácil e rápida de entender.
- A regra da afirmação única é uma boa orientação.
- Mas não tem problema em colocar mais de uma afirmação em um teste.
### Um único conceito por teste
- é desejavel ter um único conceito em cada função de teste.
- evitar funções longas que saiam testando várias coisas uma após a outra.
### F.I.R.S.T
- Testes limpos seguem outras cinco regras:
- Rapidez (Fast): Os testes devem ser rápidos.
- Independência (Independent): Os testes não devem depender uns dos outros. 
- Repetitividade (Repeatable): Deve-se poder repetir os testes em qualquer ambiente.
- Autoavaliação (Self-Validating): Os testes devem ter uma saída booleana. Obtenham ou não sucesso. 
- Pontualidade (Timely): Devemos criar os testes de unidade imediatamente antes do código de produção no qual serão aplicados.

### Conclusão
- Os testes são tão importantes para a saúde de um projeto quanto o código de produção.
- Eles preservam e aumentam a flexibilidade, capacidade de manutenção e reutilização do código de produção.
- Manter os testes sempre limpos. Se deixar os testes se degradarem, o código também irá.
