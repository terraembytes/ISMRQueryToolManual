# Manual da Ferramenta ISMR Query Tool

O Manual de Utilização da Ferramenta ISMR Query Tool é um guia abrangente projetado para ajudar os usuários a entender e utilizar efetivamente 
todas as funcionalidades e recursos oferecidos pela mesma. Este manual é destinado a todos os usuários, desde iniciantes 
até avançados, e oferece instruções passo a passo para usufruir de tudo que ela pode nos oferecer.

## 🛠️ Construído com

* [Markdown](https://www.markdownguide.org) - Linguagem de marcação utilizada 
* [Mkdocs](https://www.mkdocs.org) - Gerador de site à partir de arquivos MarkDown

# Para colaboradores

> Abaixo serão disponibilizadas instruções para que os colaboradores do projeto possam clonar e fazer um deploy atualizado do Manual

### Pré-Requisitos (Este guia utiliza como editor o VS Code)

* [Python 3.x](https://www.python.org)
* [GitHub CLI](https://git-scm.com/downloads)

### Preparando o ambiente (GitHub CLI)

1. Execute o git clone da branch **main**

   ```
   git clone https://github.com/terraembytes/ISMRQueryToolManual.git
   ```
   
2. Agora, para criar o ambiente virtual python, execute dentro do repositório que foi clonado:

   ```
   python -m venv venv
   ```

3. Ativando o ambiente virtual para a instalação do mkdocs:

   ```
   source venv/Scripts/activate
   ```

4. Instalando a biblioteca MkDocs no ambiente virtual:

   ```
   pip install mkdocs-material
   ```

### Realizando as alterações no projeto (VS Code)

1. Depois de realizar as alterações, um preview do deploy do projeto pode ser visto executando o seguinte comando no terminal do VS Code:

   ```
   mkdocs serve
   ```
   > O console irá fornecer um link de deploy local

2. Após verificar e realizar todas as alterações, basta executar o push do repositório atualizado no github e o deploy no github pages será executado automaticamente pelo arquivo **./github/workflows/ci.yml** no link: [Manual](https://terraembytes.github.io/ISMRQueryToolManual/).

   ```
   git add .
   git remote -v
   git commit -m $'*mensagem do commit'
   git push origin main
   ```
