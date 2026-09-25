# SEPLAG 2: Hub de Sistemas da COFIP / CAEXF

Versão de teste do [Portal SEPLAG](https://github.com/marceloclr/seplag), com uma tela de login alternativa.

**Endereço:** https://marceloclr.github.io/seplag2/

## Diferenças em relação ao portal oficial

- A tela de senha não tem mais o corredor de data center desenhado em canvas. Fica só o fundo azul-noite em degradê (CSS).
- A barra da janela de terminal (antes `root@sysboot: ~/login`) mostra **Hub de Sistemas da COFIP / CAEXF**. O texto digitado no boot passa a ser: *Coordenadoria Especial de Gestão Financeira e de Projetos - COFIP*, *Célula de Acompanhamento da Execução Financeira - CAEXF* e *Soluções de Gestão Financeira e Projetos*.

- O box ficou mais largo (640 px) para as linhas não quebrarem, e os campos se chamam *usuário* e *senha*.
- O box pulsa sem parar, alternando vermelho, amarelo, verde e o azul original (2,5 s por cor, ciclo de 10 s). O pulso continua durante a digitação e só some durante o tremor de erro e o pulso verde de acerto.

- **Tema claro como padrão, em dois tons:** fundo em meio-tom ardósia-lavanda, com as bolhas do cabeçalho do portal (verde-água, violeta, laranja, índigo) à deriva e uma malha de pontos de papel quadriculado, e box branco elevado, com sombra em camadas e a faixa em degradê da barra do portal no topo. O botão de tema (sol/lua) aparece no canto da tela de senha e continua na barra do portal. A escolha fica guardada no `localStorage` (chave `gfp.portal`), a mesma que o portal já usava. As cores do box e do pulso vêm dos tokens do tema claro do portal (`--tinta`, `--foco`, `--ok`, `--erro`, `--alerta`). Quando um token não alcança o contraste de 4,5:1 sobre o branco, usa-se um tom mais fechado da mesma cor. O tema escuro não mudou.

Todo o resto é igual ao `index.html` oficial: efeitos, animações, paleta, fontes, senha, abas e sistemas cadastrados. Para detalhes de funcionamento, veja o README do [seplag](https://github.com/marceloclr/seplag#readme).
