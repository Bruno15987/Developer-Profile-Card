# 🌐 Developer Profile Card

Página de perfil pessoal estilo **Link in Bio**, com visual cyberpunk, efeito Matrix, animações, música do YouTube, contador de visualizações, tema claro/escuro e muita personalização.

---

## ✨ Demonstração

🔗 **[Ver página ao vivo](https://bruno15987.github.io/bruninh/)**

---

## 🚀 Funcionalidades

* 🟢 Efeito Matrix + estrelas no fundo, podendo ser desligado
* 💎 Card com glassmorphism
* 👤 Foto de perfil com status online
* ⌨️ Efeito de digitação no nome e na frase
* 🔄 Frases que trocam automaticamente
* 🌅 Saudação automática: Bom dia / Boa tarde / Boa noite
* 🕐 Horário em tempo real
* 👁️ Contador de visualizações único por dispositivo
* 🎵 Música de fundo via link do YouTube
* 🔓 Overlay "Clique para entrar" para desbloquear a música
* 🌗 Tema claro / escuro com memória
* 🖱️ Cursor personalizado: normal, trilha ou imagem
* ✨ Partículas no avatar
* 💓 Pulsação do avatar e das letras quando a música toca
* 🎨 Cor de destaque personalizável
* 🖼️ Fundo com imagem opcional
* 🕘 Exibição da última visita
* 📤 Botão de compartilhar
* 📱 Totalmente responsivo
* ⚙️ Configuração fácil pelo arquivo `config.js`

---

## 📸 Preview

O projeto foi desenvolvido para funcionar como uma página pessoal moderna, combinando estética **cyberpunk**, **glassmorphism**, efeitos neon e elementos interativos.

---

## 📁 Como usar este projeto

### 1. Faça um Fork ou clone o projeto

Você pode:

* Clicar em **Fork** neste repositório; ou
* Baixar o projeto em `.zip` e extrair na sua pasta.

Depois, abra a pasta do projeto.

---

### 2. Personalize o `config.js`

Todas as principais configurações do perfil ficam centralizadas no arquivo `config.js`.

Exemplo:

```js
const CONFIG = {
    // Informações principais
    nome: "Seu Nome",
    frase: '"Sua frase motivacional aqui."',
    badge: "💻 Programador",
    dataAtualizacao: "Atualizado em 22/08/2026",

    // Frases extras
    // Elas podem trocar automaticamente no perfil
    frases: [
        '"Frase 1"',
        '"Frase 2"',
        '"Frase 3"'
    ],

    // Visual
    corDestaque: "#79C83D",
    fotoPerfil: "favicon.jpeg",
    favicon: "favicon.jpeg",
    fundoImagem: "",
    efeitosFundo: true,

    // Cursor
    // Opções: "normal" | "trilha" | "imagem"
    tipoCursor: "normal",
    cursorImagem: "cursor.png",

    // Música do YouTube
    musica: "https://www.youtube.com/watch?v=SEU_VIDEO_ID",

    // Redes sociais
    redes: [
        {
            nome: "GitHub",
            link: "https://github.com/seuusuario",
            icone: "fa-brands fa-github"
        },
        {
            nome: "YouTube",
            link: "https://youtube.com/@seucanal",
            icone: "fa-brands fa-youtube"
        },
        {
            nome: "Instagram",
            link: "https://instagram.com/seuuser",
            icone: "fa-brands fa-instagram"
        }
    ],

    // Contador de visualizações
    contadorChave: "seu-nome-perfil-v1",
    contadorStorage: "seu_nome_visited_v1"
};
```

### 🔧 Principais configurações

| Configuração      | Função                                    |
| ----------------- | ----------------------------------------- |
| `nome`            | Nome exibido no perfil                    |
| `frase`           | Frase principal                           |
| `badge`           | Badge abaixo do nome                      |
| `frases`          | Frases que podem alternar automaticamente |
| `corDestaque`     | Cor principal dos efeitos                 |
| `fotoPerfil`      | Foto do perfil                            |
| `favicon`         | Ícone da página                           |
| `fundoImagem`     | Imagem de fundo                           |
| `efeitosFundo`    | Ativa/desativa Matrix e estrelas          |
| `tipoCursor`      | Define o tipo de cursor                   |
| `cursorImagem`    | Imagem usada pelo cursor                  |
| `musica`          | Link do vídeo do YouTube                  |
| `redes`           | Redes sociais exibidas                    |
| `contadorChave`   | Identificação do contador                 |
| `contadorStorage` | Identificação do armazenamento local      |

---

## 📂 Arquivos importantes

| Arquivo         | Função                  |
| --------------- | ----------------------- |
| `index.html`    | Página principal        |
| `config.js`     | Configurações do perfil |
| `favicon.jpeg`  | Foto do perfil          |
| `manifest.json` | Configuração do PWA     |
| `sw.js`         | Service Worker e cache  |
| `README.md`     | Documentação do projeto |

---

## 🛠️ Publicar no GitHub Pages

### Primeira publicação

Abra o terminal dentro da pasta do projeto:

```bash
git init
git add .
git commit -m "Primeira versão do meu perfil"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

Depois, no GitHub:

**Settings → Pages → Build and deployment → Source → Deploy from a branch**

Selecione:

```text
Branch: main
Folder: / (root)
```

Clique em **Save**.

Após alguns instantes, o GitHub Pages disponibilizará o site.

---

## 🔄 Atualizar o projeto

Depois de fazer alterações:

```bash
git add .
git commit -m "Atualização do perfil"
git push
```

No **CachyOS / Linux**, esses mesmos comandos funcionam normalmente.

---

## 📦 Estrutura do projeto

```text
📦 Developer-Profile-Card
 ┣ 📜 index.html
 ┣ 📜 config.js
 ┣ 🖼️ favicon.jpeg
 ┣ 📜 manifest.json
 ┣ 📜 sw.js
 ┗ 📜 README.md
```

---

## 🎨 Personalização

### Alterar a cor

No `config.js`:

```js
corDestaque: "#79C83D",
```

Você pode trocar por qualquer cor hexadecimal.

Exemplo:

```js
corDestaque: "#00ffff",
```

---

### Desativar os efeitos de fundo

Para remover o Matrix e as estrelas:

```js
efeitosFundo: false,
```

Para ativar novamente:

```js
efeitosFundo: true,
```

---

### Alterar o cursor

Cursor normal:

```js
tipoCursor: "normal",
```

Cursor com trilha:

```js
tipoCursor: "trilha",
```

Cursor usando uma imagem:

```js
tipoCursor: "imagem",
cursorImagem: "cursor.png",
```

---

### Alterar a música

Use um link de vídeo do YouTube:

```js
musica: "https://www.youtube.com/watch?v=SEU_VIDEO_ID",
```

A música é desbloqueada pelo overlay **"Clique para entrar"**, pois os navegadores normalmente bloqueiam reprodução automática de áudio.

---

## 👁️ Contador de visualizações

O projeto possui um sistema para identificar visualizações únicas por dispositivo.

Exemplo:

```js
contadorChave: "bruninh-profile-v1",
contadorStorage: "bruninh_visited_v1",
```

### ⚠️ Importante

Se você criar uma nova versão do contador, altere essas duas chaves para evitar conflitos com versões anteriores.

Exemplo:

```js
contadorChave: "bruninh-profile-v2",
contadorStorage: "bruninh_visited_v2",
```

---

## 📱 Responsividade

O projeto foi desenvolvido para funcionar em diferentes tamanhos de tela:

* 💻 Computadores
* 🖥️ Monitores
* 📱 Celulares
* 📲 Tablets

É recomendado testar o perfil em pelo menos um computador e um celular antes de publicar alterações importantes.

---

## 💡 Dicas

* Mantenha a `fotoPerfil` em formato quadrado para obter um resultado melhor.
* Evite imagens de fundo muito pesadas.
* Use uma imagem de cursor pequena.
* Sempre teste os links das redes sociais.
* Verifique se o link do YouTube está correto.
* Faça `git add`, `git commit` e `git push` sempre que atualizar o projeto.
* Se alterar o contador, atualize `contadorChave` e `contadorStorage`.
* Teste o site em dispositivos móveis.
* O arquivo `config.js` concentra grande parte da personalização do projeto.

---

## 🧠 Créditos

Feito com ❤️ por **Bruninh**.

Projeto inspirado em páginas modernas de **Link in Bio**, combinando elementos de cyberpunk, Matrix, glassmorphism e interfaces futuristas.

---

## 📄 Licença

Este projeto é livre para uso pessoal e educacional.

Você pode modificar, personalizar e utilizar o projeto conforme suas necessidades.
