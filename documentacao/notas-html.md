-> Aprendizagem e ultilização do elemento HTML input. Sendo que ele tem três atributos: como type (que é a tipagem) o name (que é o nome do evento, ele é importante para enviar posteriormente o dado que foi preeenchido nesse input pelo ususário, ao banco de dados no back-end, é referente ao valor dentro do campo) e o id (que é o idenficador único da tag, que se ultilizado também pelo CSS e futuramente pelo JavaScript).

Outros tipos de input:

* input do type password: está relacionado a inclusão de senhas, ele ficará camuflado no momento em que o usuário está digitando a senha, há um botão na lateral caso queira ver oque foi digitado.

* input do type number: está relacionado a inclusão apenas de números, não aceita letras ou outros caracteres, há duas setas na lateral, sendo que a de cima aumenta a contagem e a de baixo diminui a contagem da numeração.

* input do type email: está relacionado a inclusão de dados em formato de email, tendo algumas obrigações como a inclusão de @ no decorrer da digitação.

* input do type checkbox: está relacionado a um pequeno quadrado para marcação de conferência. 

* input do type submit: é do tipo que irá enviar o formulário que foi preenchido. Ele tem o atributo value que refebe o valor de pesquisar.

* input do type hidden: é do tipo input escondido para as pessoas que estão vendo o formulário, dentro do formulário.

-> A tag label é do tipo inline (o elemento inline, ele permite os elementos fiquem na linha, ocupando somente o espaço do conteúdo e não faz quebra de linha/não joga o próximo elemento para baixo, e não ocupa 100% da linha que tem de espaço) e a tag input é inline-block (ele faz com que o campo continue com as suas propriedade inline em termos de tamanho dele, porém destrava umas propriedade de bloco).
  Exemplo: 
          a propriedade width, não é liberada no tipo inline, mas ele é habilitável no tipo inline-block  (assim, ele será redirecionado para a proxima linha e poderá preeencher a largura da linha toda).

-> Geralmente o input está acompanhado de uma label, que é um elemento HTML. Ele serve para duas coisas muito importantes: primeiro escrever qual é a especificação do campo (ex: título principal) e a segunda funcionalidade é para a acessibilidade. Ele terá um atributo do tipo for, como o mesmo nome que o id do input relacionado a ele, para facilitar ao leitor de tela, na questão da acessibilidade entender a referente ao input, e faz a relação delas estarem interligadas. Na ultilização do for, ao clicar no título, ele automaticamente já direciona o cursor para dentro do input.

* -> Para aplicação de fonte dentro de input, button, select, textarea: ele não pega direto o que foi definido no body, sempre precisa informar.

-> A tag select é um tipo de campo para selecionar opções. Sendo que ele tem dois atributos: o name (que é o nome do evento, ele é importante para enviar posteriormente o dado que foi preeenchido nesse input pelo usuário, ao banco de dados no back-end, é referente ao valor dentro do campo) e o id (que é o idenficador único da tag, que se ultilizado também pelo CSS e futuramente pelo JavaScript). 

-> Dentro da tag select é muito ultilizada a tag option, que ao incluir no value os dados como (music, movie, etc), ficará uma lista pre definida com os valores do dados descritos anteriormente.

-> A tag textarea que é o campo para inclusão de conteúdo. Sendo que ele tem quatro atributos: o name (que é o nome do evento, ele é importante para enviar posteriormente o dado que foi preeenchido nesse input pelo ususário, ao banco de dados no back-end, é referente ao valor dentro do campo), o id (que é o idenficador único da tag, que se ultilizado também pelo CSS e futuramente pelo JavaScript), o cols (que se refere ao tamanho, que é a quantidade de colunas) e o rows (que se refere ao tamanho, que é a quantidade de linhas). OBS: O cols e o rows normalmente é definido pelo CSS e não pelo HTML, então podemos apagar estes elementos nessa tag, ficando apenas o name e o id.

-> A tag form, é ultilizada para a criação de formulários. Dento da tag form colocamos as tags dos inputs. Sendo que ele tem primariamente dois atributos: o action (que irá dizer para onde/local o formulários será enviado, ao clincar no botão de enviar) e o method (temos dois tipos de métodos, definidos pelo protocolo HTTP, ele tras um conjunto de regras que defini alguns verbos/metodos para a comunicação, que são eles o GET (que é ultilizado para Receber e Enviar recursos/dados pela URL) e o POST (é ultilizado para Enviar recursos/dados pelo CORPO DA REQUISIÇÃO/REQUEST). 
Quando não informamos o método em um formulário, por padrão ele coloca o GET, e quando não definimos a action, ele ultiliza a mesma página para atualizar e fica na mesma página).

-> A tag fieldset, é ultilizada para fazer um conjunto/agrupamento de campos dentro de uma tag form de formulário. -> E a tag legend, é ultilizada dentos da tag fieldset. A tag legend já vem com uma estilização padrão do navegador de borda de formulário.

    /*No CSS -> Para tirar a borda de configuração padrão da tag do HTML*/
    fieldset {
      border: none; 
    }

* Quando se quer transformar em um campo do formulário com o preenchimento obrigatório, temos a propriedade/atributo no HTML -> riquered.
  E no CSS podermos configurar qual será as propriedade para quando esse evento for chamado.
  input:invalid {
  border: 1px solid #FF1010;
}