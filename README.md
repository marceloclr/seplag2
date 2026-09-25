# SEPLAG 2: Hub de Sistemas da COFIP / CAEXF

Versão de teste do [Portal SEPLAG](https://github.com/marceloclr/seplag), com uma tela de login alternativa.

**Endereço:** https://marceloclr.github.io/seplag2/

## Diferenças em relação ao portal oficial

- A tela de senha não tem mais o corredor de data center desenhado em canvas. Fica só o fundo azul-noite em degradê (CSS).
- A barra da janela de terminal (antes `root@sysboot: ~/login`) mostra **Hub de Sistemas da COFIP / CAEXF**. O texto digitado no boot passa a ser: *Coordenadoria Especial de Gestão Financeira e de Projetos - COFIP*, *Célula de Acompanhamento da Execução Financeira - CAEXF* e *Soluções de Gestão Financeira e Projetos*.

- O box ficou mais largo (640 px) para as linhas não quebrarem, e os campos se chamam *usuário* e *senha*.
- O box pulsa sem parar, alternando vermelho, amarelo, verde e o azul original (2,5 s por cor, ciclo de 10 s). O pulso continua durante a digitação e só some durante o tremor de erro e o pulso verde de acerto.

- **Proposta de paleta clara na tela de senha:** fundo branco-azulado com halos suaves de índigo e verde-água, janela branca translúcida, textos em verde 700 e azul 700 e o mesmo pulso de quatro cores, em tons mais fortes. Layout, fontes, efeitos e tempos são os mesmos da versão escura em produção. As cores ficam num bloco próprio no CSS (*Paleta clara*); apagar o bloco devolve a versão escura.

Todo o resto é igual ao `index.html` oficial: efeitos, animações, paleta, fontes, senha, abas e sistemas cadastrados. Para detalhes de funcionamento, veja o README do [seplag](https://github.com/marceloclr/seplag#readme).
