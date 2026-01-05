# Manifesto Apologético do Formato Universal

## Um Formato para Durar no Tempo

O [Unicode Standard](https://en.wikipedia.org/wiki/Unicode) foi uma revolução ao transcender as limitações das codificações de caracteres tradicionais como o ASCII, pois o Unicode suporta caracteres além dos 128 disponíveis no inglês, o que o torna universal. O formato [UTF-8](https://en.wikipedia.org/wiki/UTF-8) tornou-se uma implementação magistral do padrão Unicode, mantendo compatibilidade retroativa com o ASCII. Na verdade, o ASCII agora é um subconjunto do UTF-8.

Isso é relevante porque o formato ASCII resistiu ao teste do tempo e é considerado um dos melhores formatos para armazenar textos eletrônicos (etexts) com a intenção de durabilidade. A maioria dos romances, livros, contos e histórias em domínio público disponíveis no [Projeto Gutenberg](https://www.gutenberg.org) está em formato UTF-8.

Nas palavras do Projeto Gutenberg:[^1]

> O ponto principal de tudo isso é que, anos à frente, os textos eletrônicos do Projeto Gutenberg ainda serão viáveis, mas programa após programa, sistema operacional após sistema operacional vão acabar como os dinossauros — assim como todo o hardware que os roda. Claro que isso vale para todos os etexts em ASCII simples... não apenas aqueles que você conseguiu acessar do Projeto Gutenberg. A questão é que daqui a uma década provavelmente não teremos os mesmos sistemas operacionais, nem os mesmos programas, e portanto todos os vários tipos de etexts que não forem ASCII simples estarão obsoletos. Precisamos ter etexts em arquivos que um programa leitor/pesquisador de ASCII simples consiga lidar; isso não quer dizer que nunca deve haver marcação... apenas que as formas de marcação devem ser facilmente conversíveis em arquivos ASCII simples, para que sua utilidade não expire quando os programas deixarem de existir. Lembra de toda a dor de cabeça com programas CONVERT para transformar arquivos de processadores de texto antigos em ASCII simples?

## Markdown

É claro que o Projeto Gutenberg só aceita [texto simples](https://en.wikipedia.org/wiki/Plain_text) (arquivos .txt em UTF-8), mas o [Markdown](https://en.wikipedia.org/wiki/Markdown) é uma linguagem de marcação que é essencialmente texto simples — ou seja, continua legível em qualquer editor de texto puro.

Markdown é uma linguagem de marcação leve, com sintaxe simples, discreta e legível por humanos. Foi criada para ser fácil de escrever em qualquer editor de texto genérico e fácil de ler em sua forma bruta. Na verdade, é tão simples e não intrusiva que alguém pode abrir um arquivo Markdown (com extensão ".md") e lê-lo quase como se fosse um "arquivo ASCII simples". Você pode até renomear a extensão para ".txt" se preferir. No Windows, basta usar o Bloco de Notas. No Linux, editores de texto puro não faltam: gedit (e variantes), Kate, Emacs, Vim, Nano, etc.

Nesse sentido, o Markdown se alinha perfeitamente com o princípio do Projeto Gutenberg: a marcação deve ser facilmente conversível e não deve comprometer a legibilidade ou a durabilidade do texto. O Markdown consegue isso precisamente por ser texto simples e uma marcação não intrusiva.

## Uma Linguagem Intercambiável

Arquivos escritos em UTF-8 usando a linguagem Markdown não são apenas fáceis de ler e abrir em qualquer sistema operacional ou editor de texto puro, mas também fáceis de converter para formatos profissionais ou mais complexos.

A maneira mais fácil de fazer isso é importar seu conteúdo diretamente em um processador de texto como o **LibreOffice** ou **Microsoft Office**, ou em editores de editoração como **Scribus** ou **Adobe InDesign**.

No entanto, o programa [Pandoc](https://pandoc.org/) está disponível para vários sistemas operacionais — Windows, Linux, BSD, macOS etc. Ele permite converter de e para muitos formatos diferentes. E é gratuito e de código aberto.

Claro, o Pandoc é uma ferramenta de linha de comando, feita para ser usada no Prompt de Comando, PowerShell, terminal do Linux etc. Mas é tão simples quanto digitar:

```console
$ pandoc teste.md -f markdown -t docx -s -o teste.docx
```

O nome do arquivo `teste.md` diz ao Pandoc qual arquivo converter. A opção `-s` o instrui a criar um arquivo "autônomo", com cabeçalho e rodapé, em vez de apenas um fragmento. O parâmetro `-o teste.docx` especifica que a saída deve ir para `teste.docx`. Note que poderíamos ter omitido `-f markdown -t docx`, já que o Pandoc é esperto o suficiente para inferir os formatos a partir dos nomes dos arquivos — mas não custa incluí-los.[^2]

A aparência geral do arquivo convertido é excelente — não há realmente nada do que reclamar.

27 de julho de 2023 (_revisado em 17 de julho de 2025_)

Daniel Dias Rodrigues

[^1]: Michael Hart, "The History and Philosophy of Project Gutenberg", *Project Gutenberg*, Agosto de 1992, [https://www.gutenberg.org/about/<wbr>background/history\_and\_<wbr>philosophy.html](https://www.gutenberg.org/about/background/history_and_philosophy.html#the-project-gutenberg-philosophy-continued-2).

[^2]: "Getting started with pandoc. Step 6: Converting a File", *Pandoc*, acessado em 27 de Julho de 2023, https://pandoc.org/getting-started.html#step-6-converting-a-file.