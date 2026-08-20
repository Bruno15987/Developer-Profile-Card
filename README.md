# 🌐 Bruninh Profile

Uma página de perfil moderna (Link in Bio) com visual cyberpunk, efeito Matrix, música, contador de visualizações e várias interações.

---

## ✨ Demonstração

🔗 **[Ver página ao vivo](https://bruno15987.github.io/bruninh/)**

---

## 🚀 Funcionalidades

- Efeito Matrix + estrelas no fundo
- Card com glassmorphism e grain
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
- Easter egg secreto
- Totalmente responsivo

---

## 📁 Como usar este projeto

### 1. Faça um Fork ou baixe o código

Clique em **Fork** neste repositório  
**ou** baixe o ZIP e extraia na sua pasta.

### 2. Personalize as informações

Abra o arquivo `index.html` e altere:

| O que mudar               | Onde encontrar                          |
|---------------------------|-----------------------------------------|
| Seu nome                  | No JavaScript (efeito de digitação)     |
| Sua foto                  | `src="favicon.jpeg"`                    |
| Sua frase                 | No efeito de digitação (JavaScript)     |
| Links das redes sociais   | Dentro de `.social-icons`               |
| Nome do arquivo da música | `src="sua-musica.mp3"`                  |

### 3. Coloque sua música

Coloque o arquivo da música na mesma pasta do `index.html`  
e renomeie para `sua-musica.mp3`  
(ou altere o nome no código).

### 4. Coloque sua foto

Substitua o arquivo `favicon.jpeg` pela sua foto de perfil  
(recomendado: formato quadrado).

### 5. Publique no GitHub Pages

1. Crie um repositório no GitHub
2. Envie os arquivos
3. Vá em **Settings → Pages**
4. Em **Source** escolha a branch `main`
5. Clique em **Save**

Pronto! Sua página estará no ar.

---

## 🛠️ Comandos Git (primeira vez)
git init
git add .
git commit -m "Primeira versão do meu perfil"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
text> Substitua `SEU-USUARIO` e `SEU-REPOSITORIO` pelos seus dados reais.

---

## 🎨 Como personalizar mais

### Mudar a chave do contador

Procure por estas linhas no JavaScript:
const counterKey = 'bruno15987-bruninh-v3';
const storageKey = 'bruninh_visited_v3';
textTroque por um nome único (ex: `seu-nome-perfil-v1`).

### Mudar as cores

As cores principais estão no início do CSS (`:root`).

### Remover alguma função

Basta apagar a parte correspondente no HTML ou JavaScript.

---

## 📌 Estrutura de arquivos
📦 seu-repositorio
┣ 📜 index.html
┣ 📜 favicon.jpeg      ← sua foto
┣ 📜 sua-musica.mp3    ← sua música
┗ 📜 README.md
text---

## 💡 Dicas

- Use uma música leve (mp3) para não deixar a página pesada
- Teste no celular também
- O contador só aumenta 1 vez por dispositivo (graças ao localStorage)
- O volume funciona tanto no computador quanto no celular

---

## 🧠 Créditos

Feito com ❤️ por **Bruninh**

Inspirado em páginas de Link in Bio modernas com visual cyberpunk.

---

## 📄 Licença

Este projeto é livre para uso pessoal e educacional.  
Pode modificar e usar como quiser.
