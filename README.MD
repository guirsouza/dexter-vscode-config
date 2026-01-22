# Configuração do VSCode

Durante os estudos de Frontend com React + Tailwind + Next.JS, dentro outros, fiz algumas configurações que podem ser úteis para quem estiver começando, para
facilitar o uso do VSCode.

Principalmente porquê eu tive que fazer essa configuração para todos os projetos que eu estava fazendo, uma vez que adicionava um launcher ou configuraçãos
diferente no projeto, precisava lembrar de replicar para os demais.

## Como usar

Para utilizar esse pacote é preciso instalar como se fosse uma dependência do projeto:

```bash
$ npm install git+https://github.com/guirsouza/dexter-vscode-config.git
```

Dentro do arquivo de configuração 'package.json', adicione o seguinte:

```json
"scripts": {
  "sync-config": "cp -r node_modules/@dexter/config/.vscode . && cp node_modules/@dexter/config/.gitignore ."
}
```

A pasta do .vscode fica dentro do 'node_modules' e precisa ser traziada para o projeto, desta forma, sempre que instalar ou atualizar o projeto, será preciso
executar:

```bash
$ npm run sync-config
```

Para que os arquivos mais recentes sejam usados.
