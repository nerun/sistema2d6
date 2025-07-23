# Como ler arquivos markdown

No Windows, você pode ler arquivos Markdown (`.md`) de várias formas:


## 📝 1. Bloco de Notas ou qualquer editor de texto

* Renomeie o `.md` pra `.txt`.
* Você vai ver as marcações (`#`, `**`, `-`, etc.), mas nada de formatação
visual.
* Na verdade, este arquivo é um markdown...


## 🧩 2. Plugins para navegadores

* Extensões como "Markdown Viewer" para Chrome ou Firefox permitem abrir
arquivos `.md` direto no navegador como se fossem páginas web.

🔗 Chrome [Markdown Viewer](https://chromewebstore.google.com/detail/markdown-viewer/ckkdlimhmcjmikdlpkmbgfkaikojcbjk)

🔗 Firefox [Markdown Viewer](https://addons.mozilla.org/pt-BR/firefox/addon/markdown-viewer-chrome/)


## 🌐 3. Leitores online

* Basta arrastar o `.md` pro navegador em sites como:

  * [StackEdit](https://stackedit.io/)
  * [Dillinger](https://dillinger.io/)

Ideal pra quem não quer instalar nada.


## 🪟 4. Visual Studio Code (VS Code)

* Gratuito, leve e poderoso.
* Mostra o Markdown em duas colunas: código de um lado, visual renderizado do
outro (Ctrl+Shift+V).

🔗 [Visual Studio](https://code.visualstudio.com)


## 📄 5. Converter com Pandoc

Se quiser gerar um PDF, DOCX ou HTML bonitão, use:

```console
pandoc arquivo.md -o arquivo.pdf
```

Requer o [Pandoc](https://pandoc.org/) instalado (gratuito). Ideal pra
publicação e impressão.


## 📘 5. Typora

* Editor WYSIWYG (o que você vê é o que você tem).
* Mescla visual e código num fluxo contínuo — ótimo pra ler e editar
confortavelmente.

🔗 [Typora](https://typora.io/) (é pago, mas tem teste gratuito)

