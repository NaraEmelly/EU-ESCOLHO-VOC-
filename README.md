<div align="center">

# 💌 Eu Escolho Você

### Uma cartinha romântica em uma pequena aventura retrô.

**PLAYER 1 + PLAYER 2 · AMOR: NÍVEL ∞**

Mensagens carinhosas, corações escondidos e uma trilha chiptune original, em uma experiência inspirada na nostalgia dos jogos Pokémon.

**HTML5 · CSS3 · JavaScript · Web Audio API**

</div>

---

## 🎮 Sobre o projeto

**Eu Escolho Você** é uma página interativa que transforma uma declaração de carinho em uma aventura a dois. Ao abrir a cartinha, a pessoa percorre quatro mensagens e chega a um convite especial: **“Aceita ser meu player 2?”**

O visual combina uma moldura de console, tons de rosa e lilás, arte em pixel art e animações suaves. A experiência foi pensada para ser um presente digital que pode ser personalizado com suas próprias palavras.

## ✨ O que você encontra

- 💌 **Cartinha em quatro etapas**, com mensagens e botões para continuar.
- ♥ **Três corações colecionáveis**, que revelam pequenos recados.
- 🎵 **Trilha chiptune original**, sintetizada diretamente no navegador.
- 🔊 **Controle de som**, para ativar ou desativar a música.
- ✦ **Animações de corações e estrelas** nos momentos especiais.
- 🫂 **Abraço virtual**, com uma mensagem carinhosa no final.
- 🔁 **Opção de reler a carta** sem recarregar a página.
- 📱 **Layout responsivo** para celular e computador.
- ♿ **Foco visível, rótulos nos controles e respeito à preferência por movimento reduzido.**

## 🕹️ Como funciona

1. Clique em **ABRIR CARTINHA** para iniciar a leitura e a música.
2. Avance pelas mensagens no seu ritmo.
3. Toque nos corações espalhados pela cena para descobrir os recados.
4. Aceite o convite para formar a dupla.
5. Receba um abraço virtual ou leia tudo de novo.

A coleta dos corações é opcional: você pode concluir a carta sem encontrá-los. Ao reler, os corações continuam coletados; recarregue a página para reiniciar toda a experiência.

## 🚀 Como executar

### Abrir no navegador

1. Baixe ou clone este repositório.
2. Abra `dist/index.html` no navegador.
3. Clique em **ABRIR CARTINHA**.

Se você recebeu a versão em arquivo único, abra **`eu-escolho-voce.html`**. Ela contém a mesma aplicação.

### Usar o VS Code

Abra a pasta do projeto no VS Code e sirva `dist/index.html` com uma extensão como **Live Server**, se preferir trabalhar com um servidor local.

**Não precisa de `npm install`, banco de dados, conta ou chave de API.**

> As mensagens, interações e a música funcionam sem internet. A imagem de fundo vem de um endereço externo e precisa de conexão. Se ela não carregar, a página mantém o fundo em degradê e as interações.

## 📁 Estrutura do projeto

| Arquivo | Função |
| --- | --- |
| `dist/index.html` | Página completa, incluindo estilos, mensagens, interações e áudio |
| `README.md` | Documentação do projeto |

Todo o código está concentrado no HTML. Não há uma etapa de compilação obrigatória.

## 🛠️ Tecnologias

| Tecnologia | Aplicação |
| --- | --- |
| HTML5 | Estrutura da carta e controles |
| CSS3 | Cores, layout responsivo, transições e animações |
| JavaScript | Navegação entre mensagens, coleta de corações e final interativo |
| Web Audio API | Geração da melodia e dos efeitos sonoros |

A música usa osciladores com ondas quadradas e triangulares para produzir o timbre retrô. Não depende de um arquivo MP3 e **não é uma música oficial de Pokémon**.

## 🎨 Como personalizar

Abra `dist/index.html` no editor de código.

### Mensagens da carta

Procure por `const pages`. Cada objeto representa uma das quatro etapas:

```js
{
  title: 'Oi, meu amor…',
  body: 'Escreva sua mensagem aqui.\n\nE continue em outro parágrafo.',
  button: 'CONTINUAR ▸'
}
```

Altere `title`, `body` e `button` para colocar seus próprios textos. Preserve as quatro etapas se quiser manter a lógica atual. Para adicionar ou remover etapas, ajuste também o limite de navegação e o contador em `render()`.

### Mensagem final e abraço

Procure pela função `finish()` para editar a declaração final, a assinatura e o recado do abraço virtual.

### Recados dos corações

Procure por `document.querySelectorAll('.heart')`. Os três recados estão na lista de mensagens usada dentro desse trecho.

### Cores

Edite as variáveis no bloco `:root`, no início do CSS:

```css
:root {
  --ink: #352545;
  --paper: #fff9f1;
  --pink: #f8a7c4;
  --violet: #aa94c9;
  --muted: #756280;
}
```

Alguns elementos usam cores diretamente em suas regras; ajuste-as também para uma mudança completa de paleta.

### Imagem da cena

Altere o `src` da imagem dentro de `.scene`. Para usar um arquivo local, coloque a imagem ao lado do HTML e use seu nome no `src`. Atualize também o texto alternativo (`alt`) e os créditos da arte.

## 💡 Observações

- O áudio começa após uma interação e pode ser desligado pelo botão de som.
- A música é pausada quando a aba fica oculta.
- O progresso fica apenas na página aberta; não é salvo após recarregar.
- A arte externa depende da disponibilidade do site de origem.
- A sintaxe do JavaScript foi verificada, mas a experiência visual, o áudio e o carregamento da arte ainda precisam ser conferidos no navegador de destino.

## 💖 Créditos

- **Referência visual:** jogos retrô e universo Pokémon.
- **Arte externa:** [WallpaperSafari](https://wallpapersafari.com/pokemon-pixel-phone-wallpapers/).
- **Trilha:** composição chiptune original, sintetizada pela aplicação.

Projeto de fã, sem vínculo ou endosso oficial. Pokémon e seus personagens pertencem aos respectivos titulares. Os créditos da arte não substituem uma autorização de uso.

---

<div align="center">

**Entre tantas rotas, meu lugar favorito é do seu lado. ♥**

</div>
