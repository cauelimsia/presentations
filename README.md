<div align="center">

<img src=".github/assets/deck.gif" width="820" alt="Navegação pelo deck de nutrição e estilo de vida">

# Nutrição & Estilo de Vida

**Deck web sobre saúde com engine de slides data-driven em ES modules**

<a href="#"><img height="34" src="https://img.shields.io/badge/ES_Modules-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript"></a>
<a href="#"><img height="34" src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5"></a>
<a href="#"><img height="34" src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white" alt="CSS3"></a>
<a href="https://cauelimsia.github.io/presentations/"><img height="34" src="https://img.shields.io/badge/GitHub_Pages-222222?style=flat&logo=githubpages&logoColor=white" alt="GitHub Pages"></a>

**[▶ Abrir a apresentação](https://cauelimsia.github.io/presentations/)** · [Como funciona](#-como-funciona) · [Navegação](#-navegação) · [Rodar local](#-rodar-local)

`Cada slide é um objeto` · `Sem framework` · `Sem build`

</div>

---

## 🥗 O que é

Apresentação sobre nutrição e estilo de vida, com conteúdo baseado em recomendação da OMS
(400 g de frutas e vegetais por dia, menos de 5 g de sal, açúcar livre abaixo de 10% das
calorias). Mesma engine da apresentação institucional do autor, com o conteúdo trocado.

## ⚙️ Como funciona

O deck é **data-driven**: cada slide é um objeto de dados, e a engine decide como renderizá-lo
a partir do seu tipo. Trocar o conteúdo não encosta em marcação nem em layout.

```
index.html        casco do deck (nav, footer, progress, thumbs)
app.js            engine — slides data-driven + navegação, como ES module
styles.css        tema (Poppins, pink/azul)
assets/gocare/    imagens (Pexels/Wikimedia — ver SOURCES.md)
```

> [!IMPORTANT]
> `app.js` é um **ES module**. Abrir `index.html` direto do disco (`file://`) deixa a página
> em branco — navegadores bloqueiam módulos por esse protocolo. Use um servidor local.

## ⌨️ Navegação

| Entrada | Ação |
|---|---|
| `→` `↓` `Espaço` `PgDn` | próximo |
| `←` `↑` `PgUp` | anterior |
| `Home` / `End` | primeiro / último |
| Thumbs numerados no rodapé | pular para qualquer slide |
| Hash na URL (`#5`) | deep-link por slide |

## 🚀 Rodar local

```bash
python3 -m http.server 4173
```

Depois abra `http://localhost:4173`.

## 🧱 Stack

`JavaScript (ES modules)` · `HTML5` · `CSS3` · `GitHub Pages`
