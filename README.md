# Angular Eslint + Prettier + Husky

## 1 step

fazer a migração do tslint para o eslint
para isso devemos instalar a lib **convert-tslint-to-eslint** usando o comando

```
ng add @angular-eslint/schematics
```

## 2 step

rode o comando abaixo para fazer a migração. se você usa o TSlint default gerado pela CLI do angular pode colocar sim nas perguntas

```
ng g @angular-eslint/schematics:convert-tslint-to-eslint {{YOUR_PROJECT_NAME}}

```

## 3 step

instale o prettier.

```
npm install -D prettier eslint-config-prettier eslint-plugin-prettier
```

## 4 step

no seu arquivo **.eslintrc.json** no campo extends adicione os **eslint:recommended** e o **plugin:prettier/recommended**

```
"extends": [
  "eslint:recommended",
  "plugin:prettier/recommended"
]
```

## 5 step

crie o arquivo .eslintignore e ignore os arquivos de testes

```
**/*.spec.ts
src/test.ts
```
