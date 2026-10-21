# 🌐 Developer Profile Card

Página de perfil pessoal estilo **Link in Bio**, com visual cyberpunk, efeito Matrix, animações, música por link, contador de visualizações e tema claro/escuro.

---

## ✨ Demonstração

🔗 **[Ver página ao vivo](https://bruno15987.github.io/bruninh/)**

---

## 🚀 Funcionalidades

* 🟢 Efeito Matrix + estrelas no fundo
* 💎 Card com glassmorphism
* 👤 Foto de perfil com status online
* ⌨️ Efeito de digitação no nome e na frase
* 🌅 Saudação automática: Bom dia / Boa tarde / Boa noite
* 🕐 Horário em tempo real
* 👁️ Contador de visualizações único por dispositivo
* 🗓️ "Sua última visita foi há X dias"
* 🎵 Música por link do YouTube, link direto de `.mp3` ou arquivo local
* 🌗 Tema claro / escuro
* 🖱️ Cursor personalizado (ponto que cresce sobre botões e links)
* 💬 Tooltip nos ícones sociais
* 📤 Botão de compartilhar: no celular abre o compartilhamento do sistema, no computador copia o link
* 🖼️ Preview com imagem e título quando o link é colado no WhatsApp ou no Discord
* 🥚 Easter egg: os badges aparecem quando você clica em um ícone social
* 📱 Funciona no computador e no celular
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

Exemplo com as chaves que existem de verdade:

```js
const CONFIG = {
    // Informações principais
    nome: "Seu Nome",
    frase: '"Sua frase motivacional aqui."',
    badge: "💻 Programador",
    dataAtualizacao: "Atualizado em 22/08/2026",

    // Fotos e arquivos
    fotoPerfil: "favicon.jpeg",
    favicon: "favicon.jpeg",

    // Música (veja a seção "Música" abaixo)
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
    contadorStorage: "seu_nome_visited_v1",

    // Última visita
    ultimaVisitaStorage: "seu_nome_last_visit_v1"
};
```

### 🔧 Principais configurações

| Configuração      | Função                                         |
| ----------------- | ---------------------------------------------- |
| `nome`            | Nome exibido no perfil                         |
| `frase`           | Frase escrita com efeito de digitação          |
| `badge`           | Badge abaixo do nome                           |
| `dataAtualizacao` | Texto mostrado embaixo do contador             |
| `fotoPerfil`      | Foto do perfil                                 |
| `favicon`         | Ícone da página                                |
| `musica`          | Link do YouTube, link de `.mp3` ou arquivo local |
| `redes`           | Redes sociais exibidas                         |
| `contadorChave`   | Identificação do contador                      |
| `contadorStorage` | Identificação do armazenamento local           |
| `ultimaVisitaStorage` | Identificação da data da última visita      |

---

### 🎵 Música

No `config.js`, em `musica`, você pode colar qualquer um destes:

```js
// Link do YouTube (watch, youtu.be ou shorts)
musica: "https://www.youtube.com/watch?v=SEU_VIDEO_ID",

// Link direto de um arquivo de áudio
musica: "https://exemplo.com/minha-musica.mp3",

// Arquivo local na mesma pasta
musica: "sua-musica.mp3",
```

Assim ninguém precisa baixar música pra usar o projeto — o link resolve.

Os navegadores bloqueiam áudio antes da primeira interação. Se a música não começar sozinha, **clique em qualquer lugar da página** que ela destrava.

---

## 📂 Arquivos importantes

| Arquivo         | Função                                  |
| --------------- | --------------------------------------- |
| `index.html`    | Página principal                        |
| `config.js`     | Configurações do perfil                 |
| `favicon.jpeg`  | Foto do perfil                          |
| `sua-musica.mp3`| Música local (opcional, se usar link)   |
| `README.md`     | Documentação do projeto                 |

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

---

## 📦 Estrutura do projeto

```text
📦 Developer-Profile-Card
 ┣ 📜 index.html
 ┣ 📜 config.js
 ┣ 🖼️ favicon.jpeg
 ┗ 📜 README.md
```

---

## 👁️ Contador de visualizações

O projeto possui um sistema para identificar visualizações únicas por dispositivo.

```js
contadorChave: "bruninh-profile-v1",
contadorStorage: "bruninh_visited_v1",
```

### ⚠️ Importante

Se você criar uma nova versão do contador, altere essas duas chaves para evitar conflitos com versões anteriores.

---

## 📱 Responsividade

Teste o perfil no computador e no celular antes de publicar alterações importantes.

---

## 💡 Dicas

* Mantenha a `fotoPerfil` em formato quadrado para obter um resultado melhor.
* Prefira link do YouTube a arquivo de música — não pesa no repositório.
* Se trocar o nome em `config.js`, atualize também o `og:title` no `index.html`: o WhatsApp não executa JavaScript.
* Sempre teste os links das redes sociais.
* Faça `git add`, `git commit` e `git push` sempre que atualizar o projeto.
* Se alterar o contador, atualize `contadorChave` e `contadorStorage`.
* O arquivo `config.js` concentra grande parte da personalização do projeto.

---

## 🧠 Créditos

Feito com ❤️ por **Bruninh**

Projeto inspirado em páginas modernas de **Link in Bio**, combinando elementos de cyberpunk, Matrix, glassmorphism e interfaces futuristas.

---

## 📄 Licença

Este projeto é livre para uso pessoal e educacional.

Você pode modificar, personalizar e utilizar o projeto conforme suas necessidades.
