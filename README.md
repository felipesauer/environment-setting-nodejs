
# Olá Config :wave:


Configurações básicas de ambiente em nodejs.

### Preparando ambiente

    npm init -y
    
### Instalando depenências de desenvolvimento

    npm i -D @babel/cli @babel/core @babel/node @babel/plugin-proposal-class-properties @babel/plugin-proposal-decorators @babel/preset-env @babel/preset-typescript @types/jest @typescript-eslint/eslint-plugin @typescript-eslint/parser babel-plugin-module-resolver babel-plugin-transform-typescript-metadata eslint eslint-config-prettier eslint-plugin-prettier jest pettier ts-jest ts-node ts-node-dev tsconfig-paths typescript

### Package.json config "scripts"

    "scripts": { 
	    "dev": "ts-node-dev -r tsconfig-paths/register --inspect --transpile-only --ignore-watch node_modules src/index.js",
	    "build": "babel src --extensions \".js,.ts\" --out-dir dist --copy-files",
	    "test": "jest"
	}
