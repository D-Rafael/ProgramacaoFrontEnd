# ProgramacaoFrontEnd
Atividades, projetos e anotaÃ§Ãµes da disciplina de ProgramaÃ§Ã£o Front-End (Unicesumar, 2025). ConteÃºdo abrange HTML5, CSS3 e JavaScript.

## Coisas Importantes (Leia Primeiro)

> IMPORTANTE: Se voce quer manter medidas exatas no layout, use `box-sizing: border-box;`.
> Sem isso, o elemento pode "estourar" o espaco e quebrar o alinhamento da pagina.


## Atalhos Importantes do VSCode

Tabela de apoio rapido para acelerar a escrita e edicao de codigo no dia a dia.

| Atalho | Funcao | Exemplo de uso |
|---|---|---|
| `Ctrl + Enter` | Criar linha abaixo da atual | Voce esta em uma linha de HTML e quer abrir espaco logo abaixo sem ir para o fim da linha. |
| `Ctrl + Shift + Enter` | Criar linha acima da atual | Inserir rapidamente uma linha antes de uma `<section>` ja existente. |
| `Alt + Up / Down` | Mover linha para cima/baixo | Reorganizar a ordem de estilos CSS sem recortar e colar. |
| `Alt + Shift + Down` | Duplicar linha | Duplicar uma `<div>` base para criar outro bloco semelhante. |
| `Ctrl + D` | Selecionar proxima ocorrencia igual | Selecionar uma palavra (ex.: `container`) e editar varias ocorrencias uma a uma. |
| `Ctrl + Shift + L` | Selecionar todas as ocorrencias iguais | Renomear todas as ocorrencias de uma classe CSS no arquivo de uma vez. |
| `Ctrl + /` | Comentar/descomentar linha | Testar um trecho de JavaScript sem apagar, comentando temporariamente. |
| `Shift + Alt + F` | Formatar codigo automaticamente | Corrigir indentacao e espacamento de um arquivo HTML/CSS inteiro. |
| `F2` | Renomear simbolo (variavel/funcao) | Renomear `nomeUsuario` para `userName` com atualizacao consistente. |
| `Ctrl + Space` | Abrir sugestoes/autocomplete | Ver sugestoes de propriedades CSS como `display`, `justify-content`, etc. |
| `Tab` com Emmet | Expandir abreviacoes HTML/CSS | Escrever `ul>li*3` e pressionar `Tab` para gerar a estrutura completa. |
| `Ctrl + P` | Buscar e abrir arquivos rapidamente | Abrir `Aula02/aprendizado/aprendizadodaaula.html` digitando parte do nome. |
| `Ctrl + Shift + P` | Abrir Command Palette | Executar comandos como "Format Document" ou mudar tema rapidamente. |

### Dica de estudo

Treine 2 ou 3 atalhos por semana ate virar habito. Em pouco tempo, voce ganha velocidade e fica mais focado na logica do codigo.

---
## Aula02/aprendizado/aprendizadodaaula.html
### O que esse codigo faz
Esse arquivo monta uma pagina HTML basica para treino de estrutura. Ele mostra titulos, paragrafos, botoes, partes semanticas da pagina e uma imagem. E como montar o "esqueleto" de uma casa antes de decorar.
### Detalhe por detalhe
- `<!doctype html>`: avisa ao navegador que o documento usa HTML moderno.
- `<html lang="en">`: elemento raiz da pagina; `lang` informa o idioma principal.
- `<head>`: area de configuracoes invisiveis da pagina.
- `<meta charset="UTF-8" />`: define codificacao de texto (evita letras quebradas).
- `<meta name="viewport"...>`: ajuda a pagina a ficar boa no celular.
- `<title>...</title>`: nome da aba do navegador.
- `<body>`: tudo que aparece para quem visita o site.
- `<div>`: caixa generica para agrupar conteudo.
- `<h1>`, `<h2>`, `<h3>`: niveis de titulo (do mais importante ao menos importante).
- `<p>`: paragrafo de texto.
- `<span>`: texto em linha (nao quebra para outra linha sozinho).
- `<button>`: botao clicavel.
- `<header>`, `<nav>`, `<section>`, `<main>`, `<footer>`: blocos semanticos (explicam a funcao de cada parte da pagina).
- `<img src="..." alt="...">`: mostra imagem; `alt` descreve a imagem para acessibilidade.

Exemplo comentado linha por linha (versao simplificada):
```html
<!doctype html> <!-- Diz: este arquivo usa HTML5 -->
<html lang="pt-BR"> <!-- Inicio da pagina e idioma -->
  <head> <!-- Configuracoes -->
    <meta charset="UTF-8" /> <!-- Permite acentos corretamente -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" /> <!-- Responsivo -->
    <title>Aula 2 - Front-end</title> <!-- Titulo da aba -->
  </head>
  <body> <!-- Conteudo visivel -->
    <h1>Titulo principal</h1> <!-- Titulo mais importante -->
    <p>Meu primeiro paragrafo</p> <!-- Texto comum -->
    <button>Clique aqui</button> <!-- Botao -->
    <img src="img/fotoPortifolio.png" alt="Foto de portifolio" /> <!-- Imagem com descricao -->
  </body>
</html>
```

Por que foi escrito assim:
- Comecar com HTML puro facilita entender a base antes de CSS e JavaScript.
- Repetir tags (`<p>`, `<button>`) ajuda a fixar diferenca entre blocos e elementos em linha.
- Usar tags semanticas prepara para sites reais mais organizados.
### O que eu aprendi
- Estrutura minima de uma pagina HTML.
- Diferenca entre tags de conteudo (`p`, `h1`) e organizacao (`div`, `section`, `main`).
- Importancia do `alt` na imagem para acessibilidade.
- Que semantica e como colocar "etiquetas" certas em cada comodo da casa.
### Cuidado com isso
- `lang="en"` com texto em portugues pode atrapalhar leitores de tela; melhor `pt-BR`.
- Caminho de imagem em web fica mais seguro com `/` (`img/fotoPortifolio.png`) em vez de `\`.
- Muitos paragrafos iguais sao bons para treino, mas em projeto real deve ter conteudo claro.
- Se os acentos aparecerem quebrados, revisar UTF-8 no arquivo e no editor.
---

## .vscode/settings.json
### O que esse codigo faz
Esse arquivo configura o comportamento do VSCode para o projeto. Ele define tamanho de tabulacao, formatacao automatica e regras do Prettier. E como configurar a "regua e o caderno" antes de estudar.
### Detalhe por detalhe
- `"editor.tabSize": 2`: cada tab vale 2 espacos (padrao comum em front-end).
- `"editor.fontSize": 14`: tamanho da letra no editor.
- `"editor.formatOnSave": true`: formata automaticamente ao salvar.
- `"editor.defaultFormatter": "esbenp.prettier-vscode"`: usa a extensao Prettier para formatar.
- `"prettier.singleQuote": true`: usa aspas simples quando possivel.
- `"prettier.trailingComma": "all"`: adiciona virgula final quando permitido.
- `"prettier.tabWidth": 2`: largura de indentacao no Prettier.
- `"prettier.semi": true`: coloca `;` no fim das instrucoes.
- `"[markdown]": { ... }`: configuracao especifica para arquivos Markdown.

Exemplo comentado linha por linha:
```json
{
  "editor.tabSize": 2, // Recuo padrao com 2 espacos
  "editor.formatOnSave": true, // Formata quando salvar
  "editor.defaultFormatter": "esbenp.prettier-vscode", // Define o formatador principal
  "prettier.singleQuote": true // Prefere aspas simples
}
```

Por que foi escrito assim:
- Padronizacao evita codigo "baguncado" entre arquivos.
- Autoformatar economiza tempo e reduz erro visual.
- Ter regra fixa deixa o codigo mais facil de ler por outras pessoas.
### O que eu aprendi
- Editor tambem faz parte do estudo de programacao.
- Ferramentas de formatacao ajudam a manter consistencia.
- Configuracao local do projeto melhora produtividade.
### Cuidado com isso
- O JSON oficial nao aceita comentarios; comentarios no bloco acima sao apenas didaticos.
- Se Prettier nao estiver instalado, algumas regras nao vao funcionar.
- Times diferentes podem usar padroes diferentes; alinhar com equipe quando houver.
---

## Aula02/.gitkeep
### O que esse codigo faz
Esse arquivo serve para "marcar" uma pasta vazia no Git. Como o Git nao salva pasta vazia, o `.gitkeep` resolve isso.
### Detalhe por detalhe
- Nome iniciado com ponto: arquivo oculto comum para controle tecnico.
- Conteudo vazio: o objetivo nao e texto, e apenas existir.
- Local em `Aula02/`: garante que a pasta apareca no GitHub mesmo sem outros arquivos.

Exemplo comentado linha por linha:
```text
# (arquivo propositalmente vazio)
# Ele existe so para o Git versionar a pasta.
```

Por que foi escrito assim:
- Solucao simples e muito usada em projetos.
- Evita perder estrutura de pastas no repositorio.
### O que eu aprendi
- Git versiona arquivos, nao pastas vazias.
- Um arquivo tecnico pequeno pode resolver um problema de organizacao.
### Cuidado com isso
- Quando a pasta tiver arquivos reais, o `.gitkeep` pode continuar ou ser removido.
- Nao confundir `.gitkeep` com arquivo de codigo; ele e apenas estrutural.
---

## Principais Atributos HTML

Tabela de referencia rapida com atributos muito usados em HTML.

| Atributo | Onde e comum usar | Para que serve | Exemplo |
|---|---|---|---|
| `id` | Quase qualquer tag | Identificador unico do elemento na pagina | `<section id="sobre">` |
| `class` | Quase qualquer tag | Agrupa elementos para aplicar CSS/JS | `<div class="card destaque">` |
| `src` | `img`, `script`, `iframe` | Define caminho do arquivo externo | `<img src="img/foto.png" alt="Foto">` |
| `href` | `a`, `link` | Define destino do link | `<a href="contato.html">Contato</a>` |
| `alt` | `img` | Texto alternativo da imagem (acessibilidade) | `<img src="logo.png" alt="Logo da empresa">` |
| `title` | Quase qualquer tag | Dica de texto ao passar o mouse | `<button title="Salvar alteracoes">Salvar</button>` |
| `style` | Quase qualquer tag | Aplica CSS direto no elemento (uso pontual) | `<p style="color: blue;">Texto</p>` |
| `type` | `input`, `button`, `script` | Define tipo/comportamento do elemento | `<input type="email">` |
| `name` | `input`, `select`, `textarea` | Nome do campo enviado em formularios | `<input name="email">` |
| `value` | `input`, `option`, `button` | Valor inicial ou enviado do campo | `<input value="Rafael">` |
| `placeholder` | `input`, `textarea` | Texto de ajuda dentro do campo | `<input placeholder="Digite seu nome">` |
| `required` | Campos de formulario | Torna preenchimento obrigatorio | `<input type="text" required>` |
| `disabled` | Campos/botoes | Desativa interacao do usuario | `<button disabled>Indisponivel</button>` |
| `checked` | `input` checkbox/radio | Marca opcao inicialmente | `<input type="checkbox" checked>` |
| `for` | `label` | Liga o label ao `id` de um campo | `<label for="email">Email</label>` |
| `target` | `a`, `form` | Define onde abrir o link/envio | `<a href="https://github.com" target="_blank">GitHub</a>` |

Dica: prefira sempre combinar `id` e `for` em formularios e nunca esquecer o `alt` em imagens.

---
## Importante: Tamanho Fixo no CSS e Soma de Valores

### O que acontece
Quando um elemento tem `width` ou `height` fixo, e voce adiciona `padding` e `border`, o tamanho final pode aumentar.

Isso acontece no modo padrao do CSS, chamado `content-box`.

### Exemplo simples
```css
.caixa {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
}
```

Conta da largura final:
- `200` (conteudo)
- `+ 20 + 20` (padding esquerda e direita)
- `+ 5 + 5` (borda esquerda e direita)
- Total: `250px`

### Como evitar essa soma
Use `box-sizing: border-box;`

```css
.caixa {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  box-sizing: border-box;
}
```

Com isso, os `200px` passam a incluir conteudo + padding + border.




