# Módulo 1 de ReactJS Rocket-Seat

Esse módulo é um projeto de Timer dedicado ao estudo das bases do ReactJS com Typescript.
___
### Palavras chave:
>ReactJS

## Conteúdo Programático do Módulo 1

<details style="font-size: 16px">
<summary><strong style="font-size: 18px">1. Fundamentos do Nest</strong></summary>

  ---

  + Introdução
  + Criação do projeto
  ---
</details>

## Atalhos do VSCode:

>Clique para visualizar os [Atalhos do VSCode](https://silicon-chips-f58.notion.site/VsCode-Shortcuts-Atalhos-4ced0388660c4f1c93b410765c0a44cd) no Notion.

## Principais comandos:

### Aula "Criação do Projeto"

+ `npm create vite@latest`: Cria o projeto Vite.
  > **_OBS:_** Aqui você pode encontrar a documentação do [Vite](https://vitejs.dev/guide/)
+ `npm i`: Instala as dependências para rodar o projeto.
+ `npm run dev`: Roda o projeto na porta configurada no arquivo vite.config.js. Nesse projeto está na localhost:3001.

### Recurso "Figma"

+ Protótipo de Alta Fidelidade no [Figma](https://www.figma.com/community/file/1127351821076435124)

### Aula "Styled Components"

+ `npm i styled-components`: Instala o pacote do Styled Components (CSS através do Javascript).
+ `npm i @types/styled-components -D`: Instala as declarações de tipagens do Styled Componentes para ele funcionar em conjunto com o Typescript.
  > **_OBS:_** Instalar a extensão do VSCode "jvscode-styled-components"

### Aula "Configurando o ESLint"

+ `npm i eslint -D`: Instala o ESLint
+ `npm i @rocketseat/eslint-config -D`: Instala a configuração do ESLint da Rocket Seat
+ `npx eslint src --ext .ts,.tsx`: Comando para ver os erros de ESLint.
+ `npx eslint src --ext .ts,.tsx --fix`: Comando para corrigir todos os erros de ESLint que puderem ser corrigidos automaticamente.
+ Criar um script no arquivo `package.json` para rodar o comando `npm run lint` ou `npm run lint --fix`
    >
    ```
    "scripts": {
      "lint": "eslint src --ext .ts,.tsx",
    },
    ```

### **Passo a Passo para Configuração do ESLint do Crea-GO:**

1. Excluir a pasta `node_modules`.
2. Dentro do arquivo `package.json`, excluir todas as `devDependencies` que tenham "eslint" no nome.
3. Rodar `npm i`
4. Rodar o comando: `npm install eslint@8.22.0 @typescript-eslint/eslint-plugin@5.45.0 @typescript-eslint/parser@5.45.0 eslint-plugin-prettier@4.2.1 prettier@2.7.1 --save-dev`
5. Rodar o comando: `npm i -D eslint-config-creago`
6. Exclua o arquivo `.eslint.config.js` e, se não existir, crie o arquivo ´.eslintrc.json´ e coloque no seu conteúdo:
    >
    ```
    {
      "extends": "eslint-config-creago/react"
    }
    ```
7. Alterar as configurações de usuário no `settings.json`, acrescentando:
    >
    ```
    {
      "editor.codeActionsOnSave": {
          "source.fixAll": "explicit",
          "source.fixAll.eslint": "explicit"
      },
      "eslint.format.enable": true,
      "editor.formatOnSave": true
    }
    ```
8. Instalar a extensão ESLint da Microsoft no VSCode
9. Rodar `npm run lint` para mostrar os erros.
10. Testar se `Ctrl + S` num arquivo .ts ou .tsx aplica formatação do ESLint

### Aula "React Router DOM"

+ `npm i react-router-dom`: Instala o React Router para lidar com rotas na aplicação
  > Os componentes `BrowserRouter` e `ThemeProvider` são chamados de Context Providers. Eles não tem efeito visual, mas geram um contexto para os componentes que estão dentro deles.

### Aula "Header & Layout"

+ `npm i phosphor-react`: Biblioteca de ícones.

### Aula "Controlled VS Uncontrolled"

+ Controlled: Forma de lidar com formulários salvando os inputs em estados e atualizando o componente a cada interação do usuário.
+ Uncontrolled: Forma de lidar com formulário executando funções apenas quando o usuário especifica clicando num botão, por exemplo.


## Autoria e Créditos:

+ Documentação criada com carinho e dedicação por [Júlio César Freitas](https://github.com/juliofreitasbm) a serviço do [CREA-GO](https://www.creago.org.br/).