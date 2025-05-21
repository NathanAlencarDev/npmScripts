O que são Npm Scripts?
    * Se trata de linhas de scripts criadas no arquivo "package.json" onde adicionamos uma lista de comandos npm para sere executados com apenas uma linha de comando.
Em resumo nos tras produtividade e muita agilidade de produção.

    comando "npm run <stage>"

Onde devo adicionar os meus scripts?
    No arquivo package.json no scripts fild
        "scripts": {
            "test": "echo \"Error: no test specified\" && exit 1",
            "iniciar": "node src/index.js && mkdir distScript && echo \"Scritp executado com sucesso!\" "
        },
        ** Estes foram scripts criados na aula. **

        ** Criação de scripts normalmente utilziados por empresas, não existe um padrão mas são exemplos de possiveis scritps. **
        "scripts": {
            "prebuild": "npm install && ",
            "start:dev": "node src/index.js",
            "start:watch": "node --watch src/index.js"
        }
            //? OBS: O "&&" serve para passar um novo comando na memsa linha tambem chamados de Multi Tasks
        // Explicação sobre os scripts
            "prebuild" - São comandos que devem ser executados antes de rodar o projeto pela primeira vez, carregamento de pacotes.
            "start:dev" - Este carrega o comando de inicialização do projeto em ambiente de desenvolvimento.
            "start:watch" - Comando utilizado para deixar preparado o comando watch para acompanhamento em tempo real da edição do arquivo.

            //*** ISSO NAO É UM PADRÃO DE CRIAÇÃO DE SCRIPTS APENAS IDEIAS DE COMO CRIA-LOS. EXISTEM PESSOAS E EMPRESAS QUE FORMATAM O PADRÃO DELAS. TEM EMPRESAS QUE SEPARAM AS PALAVRAS COM "-"
             JA NESTE EXEMPLO UTILIZEI ":" COMO NO CURSO.

        // Dicas para bons nomes para scripts.
            //! UTILIZAR SEMPRE PALAVRAS CHAVES PARA UMA BOA ORGANIZAÇÃO DO PROJETO: EXEMPLO > "test": "..", "test-stable": "...", "test-www": ".." ...

            start: Start the application.

            dev: Start the development server with hot reloading. build: Build the application for production.

            test: Run unit tests. test:watch: Run unit tests in watch mode. test:coverage: Generate test coverage report.

            lint: Lint the codebase. lint:fix: Fix linting errors automatically.

            format: Format code according to coding standards. clean: Clean up generated files.

            precommit: Run linting, formatting, and tests before committing code. deploy: Deploy the application to a server. analyze: Analyze the bundle size or performance of the application.

            storybook: Start Storybook for component development. storybook:build: Build Storybook for production. storybook:deploy: Deploy Storybook to a hosting service.
        