
# Olá Config :wave:


Configurações básicas de ambiente em nodejs, o mesmo é composta por algumas tecnologias.

### Preparando ambiente

    npm init -y
    
### Instalando depenências de desenvolvimento

    npm i -D @babel/cli @babel/core @babel/node @babel/plugin-proposal-class-properties @babel/plugin-proposal-decorators @babel/preset-env @babel/preset-typescript @types/bcryptjs @types/cors @types/date-fns @types/express @types/ioredis @types/jest @types/joi @types/jsonwebtoken @types/redis @types/uuid @typescript-eslint/eslint-plugin @typescript-eslint/parser babel-plugin-module-resolver babel-plugin-transform-typescript-metadata eslint eslint-config-prettier eslint-plugin-prettier jest pettier ts-jest ts-node ts-node-dev tsconfig-paths typescript

### Package.json config "scripts"

    "scripts": { 
	    "dev": "ts-node-dev -r tsconfig-paths/register --inspect --transpile-only --ignore-watch node_modules __EXEC_ARQ__",
	    "typeorm": "typeorm-ts-node-esm -d __EXEC_ARQ__",
	    "build": "babel src --extensions \".js,.ts\" --out-dir dist --copy-files",
	    "test": "jest"
	}
