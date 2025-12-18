# 🛠️ Ferramentas de Automação - Suporte Produttivo

Este repositório contém um conjunto de ferramentas desenvolvidas para automatizar tarefas repetitivas e manuais da equipe de Suporte (N1/N2) no **Produttivo**. 

O objetivo é reduzir o tempo gasto em personalizações de relatórios e configurações de Excel, minimizando erros de digitação e aumentando a produtividade.

## 🚀 Funcionalidades

O projeto consiste em uma interface central (`index.html`) que dá acesso a dois geradores específicos:

### 1. Gerador de CSS (Ocultar Itens)
Automatiza a criação de códigos CSS para ocultar múltiplos elementos sequenciais em relatórios personalizados.

* **Problema:** Ocultar 50 fotos manualmente exigia digitar `#section_4_field_1_attachment_0 { display: none; }` cinquenta vezes.
* **Solução:** O script gera o bloco de código completo em segundos, bastando informar o ID base e a quantidade desejada.

### 2. Gerador de Tags para Excel
Automatiza a criação de variáveis dinâmicas para exportação de dados em planilhas.

* **Problema:** Criar colunas para 50 fotos exigia digitar `${form_fill.fotos[0].file}`, depois `[1]`, `[2]`, etc.
* **Solução:** O script gera a lista completa das variáveis sequenciais, formatada corretamente com a sintaxe `${...}` exigida pelo sistema.

---

## 💻 Como Usar

### Acesso Online
Você pode acessar as ferramentas diretamente pelo navegador através do link:
👉 **[Clique aqui para abrir as Ferramentas](https://seu-usuario.github.io/nome-do-repositorio)**
*(Substitua este link pelo seu link real do GitHub Pages após configurar)*

### Uso Local (Opcional)
Se preferir rodar no seu computador:
1.  Baixe este repositório (Download ZIP).
2.  Extraia os arquivos.
3.  Dê um duplo clique no arquivo `index.html`.

---

## ⚙️ Tecnologias Utilizadas

* **HTML5:** Estrutura das páginas.
* **CSS3 (Bootstrap 5):** Estilização visual para uma interface limpa e responsiva.
* **JavaScript:** Lógica de programação para os loops e geração dinâmica dos textos.

---

## 📝 Exemplo de Uso

**Cenário:** Precisamos ocultar as fotos de um checklist no relatório PDF, do índice 0 ao 15.

1.  Acesse o **Gerador de CSS**.
2.  No campo **ID Base**, cole: `section_2_field_0_attachment_`
3.  No campo **Quantidade**, digite: `16`
4.  Clique em **Gerar Código CSS**.
5.  O sistema entregará o código pronto:
    ```css
    #section_2_field_0_attachment_0,
    #section_2_field_0_attachment_1,
    ...
    #section_2_field_0_attachment_15 {
        display: none !important;
    }
    ```
6.  Basta copiar e colar no modo avançado do Produttivo.

---

## 🤝 Contribuição

Sugestões de melhorias são bem-vindas! Se você tiver uma ideia para uma nova ferramenta que ajude no dia a dia do suporte:

1.  Abra uma **Issue** explicando a ideia.
2.  Ou entre em contato diretamente.

---

Desenvolvido por **[Seu Nome]** 🚀
