# SEPLAG 2 — Login Lab

Laboratório para uma versão alternativa da tela de login do [Portal SEPLAG](https://github.com/marceloclr/seplag). **É só um protótipo visual:** nenhuma senha é verificada, e qualquer senha não vazia "entra".

**Endereço:** https://marceloclr.github.io/seplag2/

## Inspiração

Gerenciadores de login do Linux:

- **GDM do RHEL 8 (GNOME 3):** barra superior com data e hora, menus de acessibilidade e de energia, lista de usuários com avatar em moldura quadrada, link "Não está na lista?" e a marca centralizada no rodapé.
- **GDM do RHEL 6:** fundo azul-noite com hexágonos desfocados (bokeh), diálogo com avatar redondo, seletor de sessão e os botões Cancelar e Entrar.
- **SLiM (Arch):** cartão translúcido e compacto sobre fundo escuro.

## Fluxo

1. **Cortina:** relógio grande, como na tela de bloqueio do GNOME. Para abrir, clique, pressione qualquer tecla ou deslize para cima.
2. **Lista de usuários:** Marcelo Correia, Administrador e Visitante, além de "Não está na lista?" (que pede o usuário).
3. **Cartão de vidro:** avatar com o anel em degradê do portal, senha com botão de mostrar/ocultar, aviso de Caps Lock e seletor de sessão (Portal completo, Saneamento, SIPOG, Modo terminal).
   - Senha vazia: a janela treme com borda vermelha.
   - Senha preenchida: "Autenticando…", pulso verde e tela de boas-vindas.
4. <kbd>Esc</kbd> volta uma etapa.

Na barra superior:

- O menu de **acessibilidade** liga ou desliga alto contraste, texto grande e fundo animado.
- O menu de **energia** tem volume, Suspender, Reiniciar e Desligar. Esses botões são só de enfeite.

O fundo é desenhado em canvas: hexágonos em várias profundidades, com desfoque proporcional e paralaxe leve com o mouse. Com `prefers-reduced-motion` ativado, o fundo fica parado.

Tudo está num único `index.html`, sem dependências além das fontes do Google.
