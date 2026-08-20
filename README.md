# 🌐 Developer Profile Card

Página de perfil pessoal estilo **Link in Bio** com visual cyberpunk, efeito Matrix, animações, música de fundo, contador de visualizações, tema claro/escuro e integração com redes sociais.

---

## ✨ Demonstração

🔗 **[Ver página ao vivo](https://bruno15987.github.io/bruninh/)**

---

## 🚀 Funcionalidades

- Efeito Matrix + estrelas no fundo
- Card com glassmorphism
- Foto de perfil com status online
- Efeito de digitação no nome e na frase
- Saudação automática (Bom dia / Boa tarde / Boa noite)
- Horário em tempo real
- Contador de visualizações **único por dispositivo**
- Música de fundo com controle de volume (funciona no celular)
- Tema claro / escuro
- Cursor personalizado
- Tooltip nos ícones sociais
- Glitch no nome ao passar o mouse
- Totalmente responsivo
- **Configuração super fácil** pelo arquivo `config.js`

---

## 📁 Como usar este projeto

### 1. Baixe ou faça um Fork

- Clique em **Fork** neste repositório  
**ou**
- Baixe o ZIP e extraia na sua pasta

### 2. Personalize tudo no arquivo `config.js`

Abra o arquivo `config.js` e altere as informações:

```js
const CONFIG = {
    // ===== INFORMAÇÕES PRINCIPAIS =====
    nome: "Seu Nome",
    frase: '"Sua frase motivacional aqui."',
    badge: "💻 Programador",
    dataAtualizacao: "Atualizado em 20/08/2026",

    // ===== FOTOS E ARQUIVOS =====
    fotoPerfil: "favicon.jpeg",
    favicon: "favicon.jpeg",
    musica: "sua-musica.mp3",

    // ===== REDES SOCIAIS =====
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
        // Descomente e preencha as redes que quiser usar
    ],

    // ===== CONTADOR INTERNO =====
    contadorChave: "seu-nome-perfil-v1",      // Mude para um nome único
    contadorStorage: "seu_nome_visited_v1"    // Mude para um nome único
};
```

### 3. Coloque sua foto e música

| Arquivo            | O que fazer                                      |
|--------------------|--------------------------------------------------|
| `favicon.jpeg`     | Substitua pela sua foto de perfil (preferencialmente quadrada) |
| `sua-musica.mp3`   | Coloque sua música de fundo com esse nome        |

### 4. Adicionar mais redes sociais

Basta descomentar (remover o `//`) e preencher no array `redes`:

```js
{
    nome: "Twitter / X",
    link: "https://x.com/seuuser",
    icone: "fa-brands fa-x-twitter"
},
{
    nome: "Discord",
    link: "https://discord.gg/seulink",
    icone: "fa-brands fa-discord"
},
{
    nome: "LinkedIn",
    link: "https://linkedin.com/in/seuuser",
    icone: "fa-brands fa-linkedin"
},
{
    nome: "TikTok",
    link: "https://tiktok.com/@seuuser",
    icone: "fa-brands fa-tiktok"
},
{
    nome: "WhatsApp",
    link: "https://wa.me/5511999999999",
    icone: "fa-brands fa-whatsapp"
},
{
    nome: "Email",
    link: "mailto:seuemail@email.com",
    icone: "fa-solid fa-envelope"
}
```

---

## 🛠️ Publicar no GitHub Pages

1. Crie um repositório no GitHub (ou use este)
2. Envie os arquivos
3. Vá em **Settings → Pages**
4. Em **Source** escolha a branch `main`
5. Clique em **Save**

Pronto! Sua página estará no ar em alguns minutos.

---

## 📦 Estrutura de arquivos

```
📦 Developer-Profile-Card
 ┣ 📜 index.html          ← Página principal
 ┣ 📜 config.js           ← 🔥 Configuração fácil (edite aqui)
 ┣ 📜 favicon.jpeg        ← Sua foto de perfil
 ┣ 📜 sua-musica.mp3      ← Sua música de fundo
 ┗ 📜 README.md           ← Este arquivo
```

---

## 🧠 Comandos Git (primeira vez)

```bash
git init
git add .
git commit -m "Primeira versão do meu perfil"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

### Atualizar depois de mudanças:

```bash
git add .
git commit -m "Atualização da configuração"
git push
```

---

## 💡 Dicas importantes

- Sempre mude as chaves `contadorChave` e `contadorStorage` para valores únicos (senão o contador fica compartilhado)
- Use músicas leves (mp3) para a página não ficar pesada
- Teste no celular também
- O contador só aumenta **1 vez por dispositivo** (usa localStorage)
- O volume da música funciona tanto no PC quanto no celular

---

## 🧠 Créditos

Feito com ❤️ por **Bruninh**

Inspirado em páginas de Link in Bio modernas com visual cyberpunk.

---

## 📄 Licença

Este projeto é livre para uso pessoal e educacional.  
Pode modificar e usar como quiser.
