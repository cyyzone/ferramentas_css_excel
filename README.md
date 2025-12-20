# 🦸‍♂️ Kit de Ferramentas 

Aqui você encontra ferramentas criadas para facilitar a nossa vida no suporte, eliminando aquelas tarefas repetitivas de ficar digitando códigos ou IDs um por um. A ideia é: menos trabalho manual, mais agilidade!

## 🔗 Acesso Rápido (Links)

Não precisa baixar nada! É só clicar nos links abaixo para abrir as ferramentas direto no seu navegador:

### 🎨 [Abrir Ocultar Campos PDF](https://cyyzone.github.io/ferramentas_css_excel/ferramentas/gerador_css.html)
> **Pra que serve?** Para quando você precisa ocultar várias fotos ou campos de uma vez no relatório PDF.

### 📊 [Abrir Gerar Tags Excel](https://cyyzone.github.io/ferramentas_css_excel/ferramentas/gerador_excel.html)
> **Pra que serve?** Para gerar aquelas tags chatas (`${...}`) de listas e fotos para o Excel, sem ter que digitar uma por uma.



### 1. Usando o Ocultar Campos PDF

Sabe quando o cliente pede para ocultar 50 fotos do checklist no relatório? Em vez de escrever 50 linhas de código, faça assim:

1.  **Pegue o ID:** Vá no relatório (inspecionar elemento) e copie o ID do primeiro item.
    * *Exemplo:* `section_4_field_1_attachment_0`
2.  **Coloque na Ferramenta:** Cole direto no campo "ID Base".
    * *O Pulo do Gato:* Pode colar com o número final mesmo! O sistema é esperto e remove o `0` (ou `15`, `99`...) automaticamente para deixar só o ID base.
3.  **Defina a Quantidade:** Quantas fotos são? Digite o número (ex: `50`).
4.  **Gerar:** Clique no botão azul.
5.  **Pronto!** O site vai criar o código prontinho. É só clicar em "Copiar" e colar lá na aba "Editar código (Avançado)" do perfil de exportação.


### 2. Usando o Gerar Tags Excel

Se você precisa configurar um relatório Excel e tem que colocar as colunas de cada foto (`[0]`, `[1]`, `[2]`...), use essa ferramenta:

1.  **Pegue a Variável:** Copie o nome da variável da lista ou foto.
    * *Exemplo:* `${form_fill.fotos_do_servico[0].file}`
2.  **Coloque na Ferramenta:** Cole direto no campo "Variável Base".
    * *Dica:* Não precisa limpar nada! O sistema entende e remove sozinho os `${ }` e os colchetes `[0]`.
3.  **Escolha a Propriedade:** O que você quer mostrar? O arquivo da foto? A legenda?
    * *Exemplo:* `.file` (imagem) ou `.title` (legenda).
4.  **Gerar:** Clique no botão verde.
5.  **Sucesso:** Ele vai gerar uma lista com todas as tags na ordem certa. Copie e cole cada linha na sua planilha Excel.



## 💡 Dica de Amigo 

**"Atualizei a ferramenta, mas continua igual!"**
Às vezes o navegador guarda uma "memória" (cache) da versão antiga. Se você notar que algo mudou mas não apareceu:
* Aperte **CTRL + F5** (no Windows)
* Ou **Command + Shift + R** (no Mac)
Isso força o navegador a carregar a versão mais novinha em folha.

---

Feito com 💙
