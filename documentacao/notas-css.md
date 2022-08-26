display: block 
  Ele preenche toda a linha e empura todos os elementos para baixo.

display: flex;
flex-direction: column;
gap: 24px;
  configuração na taga principal: para direcionar todas as tags dentro de uma principal com espaçamento.
  obs: O display:flex ele estica o elemento no eixo oposto a direção. 
      Portanto como o flex-direction: é column, 
      então o display:flex esticará todo o box/conteúdo no sentido da linha.

position: absolute
  significa que o elemento ficará sobre postos, sobre os outros elementos da mesma tag
  ela destrava as propriedades: top, left, right, bottom
    e destrava também a propriedade: z-index que é o eixo de profundidade, no caso para ficar atrás dos outros elementos da tag, precisa colocar como z-index: -1.

.page {
  width: ...px;
  margin: auto}
  só com essa informação ele já alinha os itens dentro da div com classe=page como centralizado

margin-top:
  para padronização, sempre adicionar a divisão dos elementos apenas com o ajuste da margin top, e somente no ultimo elemento incluir margin botton.

padding:
  é o preenchimento interno, sempre pegar a tag maior que tenha tags dentor para usar a referencia de preenchimento interno.

* Para gerar uma linha -> no CSS
  width: 100%;
  border-bottom: 1px solid #E6E6F0;
  padding-bottom: 16px;

* Detalhe ao config margin:
  -> No HTML
    <div class="input-wrapper">
    <label>Texto<span>obs</span></label>
    </div>
  -> No CSS
    .input-wrapper label span {
      margin-left: 12px;
  }
    Se for colocado a margin no label apenas, ele entenderá que o span está dentro do label e não irá considerar para aplicação da margin-right. 
    O correto é colocar a margin-left no span que está dentro do label. 
    Na teoria dá na mesmo, porém na pratica por estar um dentro do outro a aplicação é diferente.

box-sizing: border-box;
  é ultilizado para que o tamanho da caixa, começe a ser contada a partir da borda, e não leva em consideração o tamanho definido no padding dentro da caixa.
    Como configuração padrão para resetar as configurações do navegador, sempre ao iniciar um aplicação com CSS colocar:
      * {
          margin: 0;
          padding: 0;
          box-sizing: border-box;
      }

* -> Para aplicação de fonte dentro de input, button, select, textarea: ele não pega direto o que foi definido no body, sempre precisa informar.


* Subclass / pseudo-class: é uma palavra-chave adicionada a um seletor que especifica um estado especial  do elemento selecionado.
  Ex: :hover, :focus, :outline, :invalid, :checked...
