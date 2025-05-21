
# 🚀 NPM Scripts — Automatize seu Fluxo com Agilidade

Os **NPM Scripts** são comandos personalizados definidos dentro do arquivo `package.json` que aumentam a produtividade e simplificam tarefas comuns com uma única linha no terminal.

📌 Comando base:
```
npm run <nome-do-script>
````

---

## 🛠️ Onde adicionar?

No bloco `"scripts"` do `package.json`:

```json
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "iniciar": "node src/index.js && mkdir distScript && echo \"Script executado com sucesso!\""
}
```

✔️ Esses são exemplos simples criados durante a aula.

---

## 🧱 Estrutura Profissional (Exemplo de mercado)

```json
"scripts": {
  "prebuild": "npm install",
  "start:dev": "node src/index.js",
  "start:watch": "node --watch src/index.js"
}
```

🧩 `&&` permite a execução de múltiplos comandos em sequência.

### ✳️ O que faz cada um?

* **prebuild** — Executa tarefas preparatórias antes do build inicial.
* **start\:dev** — Inicia o app em ambiente de desenvolvimento.
* **start\:watch** — Roda o app monitorando alterações em tempo real.

> ❗ Não existe um padrão fixo de nomes. Algumas empresas usam `:` (como neste exemplo), outras usam `-` para separar palavras.

---

## 📋 Boas Práticas ao Nomear Scripts

🎯 Use nomes claros e descritivos. Exemplos comuns:

```json
"scripts": {
  "start": "Start the application",
  "dev": "Start dev server with hot reload",
  "build": "Build app for production",
  "test": "Run unit tests",
  "test:watch": "Run tests in watch mode",
  "test:coverage": "Generate test coverage report",
  "lint": "Lint the codebase",
  "lint:fix": "Fix linting errors",
  "format": "Format code",
  "clean": "Clean generated files",
  "precommit": "Run checks before commit",
  "deploy": "Deploy app to server",
  "analyze": "Analyze bundle size",
  "storybook": "Run Storybook",
  "storybook:build": "Build Storybook",
  "storybook:deploy": "Deploy Storybook"
}
```

🗂️ *Scripts organizados facilitam o entendimento, a manutenção e o onboarding de novos devs.*

---

🔁 **Automatize. Padronize. Evolua.**
Use NPM Scripts para transformar comandos repetitivos em fluxos simples e rápidos!

```
