---
title: Usar o microsoft graph Toolkit com oTron
description: Começar a usar o microsoft graph Toolkit em um aplicativo Detron.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: ad0d13ceb8a6ef12535dd635bf7eb011d765db9d
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471415"
---
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a>Usar o microsoft graph Toolkit com oTron

Este artigo descreve o processo passo a passo de usar o microsoft graph Toolkit criar um aplicativo Detron e conectá-lo ao Microsoft 365. Depois de concluir as etapas, você terá um aplicativo Detron que mostra os próximos compromissos do usuário atualmente inscrevado do Microsoft 365.

## <a name="create-an-electron-app"></a>Criar um aplicativo Detron 
Crie um novo aplicativo Detron clonando [o repositório do tiposcript](https://github.com/electron/electron-quick-start-typescript) de início rápido do sistema. Isso criará um novo aplicativo Detron usando TypeScript, o que ajudará você a escrever um código mais robusto e a evitar erros de tempo de execução.

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

Altere o diretório de trabalho para o aplicativo recém-criado e instale todas as dependências.

```cmd
cd electron-quick-start-typescript
npm install
```

Instale o pacote "@microsoft/mgt-components" que contém todos os componentes web conectados ao Microsoft Graph.

```cmd
npm i @microsoft/mgt-components
```

Instale os `@microsoft/mgt-electron-provider` `@microsoft/mgt-element` pacotes e npm também. Isso permitirá que você forneça autenticação para seu aplicativo usando o MSAL e use os componentes do Microsoft Graph Toolkit.

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

Confirme se você pode executar o aplicativo.

```cmd
npm start
```

## <a name="create-an-appclient-id"></a>Criar uma ID de aplicativo/cliente

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a>Adicionar novo registro de aplicativo no Azure AD para obter uma ID do cliente

Para criar um aplicativo no Azure Active Directory (Azure AD), você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e redirecionar o URI.

Para criar o aplicativo no Azure AD:

1. Vá para o [portal do Azure](https://portal.azure.com).
1. No menu, selecione **Azure Active Directory**.
1. No menu do Azure Active Directory, selecione **Registros de aplicativos**.
1. No menu superior, selecione o **botão Novo registro.**
1. Insira o nome do seu aplicativo; por exemplo, `My Electron-App` .
1. Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório do **Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.
1. No campo **Redirecionar URI,** no menu suspenso, selecione **Cliente público/nativo (área** de trabalho móvel &) e, no campo URL, digite `msal://redirect` .
1. Confirme as alterações selecionando o **botão Registrar.**
1. Vá para o registro do aplicativo.
1. Verifique se você está na página **Visão** Geral.
1. Na seção **Essentials,** copie o valor da propriedade **Application (client).**

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Configurar o provedor de autenticação Toolkit Microsoft Graph

### <a name="initializing-electronprovider-in-your-renderer-process"></a>Inicializando oTronProvider no processo de renderização

O responsável por se comunicar com (no processo principal) para solicitar tokens de acesso e receber informações sobre o estado assinado que é necessário para que os `ElectronProvider` `ElectronAuthenticator` componentes mgt funcionem. 

Para inicializar o arquivo , adicione o código a `ElectronProvider` seguir ao *arquivo src/renderer.ts.*
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a>Inicializando o EletrônicaAuthenticator em seu processo principal

O é responsável por configurar as variáveis de configuração para autenticação `ElectronAuthenticator` MSAL, adquirir tokens de acesso e se comunicar com `ElectronProvider` o . Inicializar o no processo principal e configurar as variáveis de configuração, como iD do cliente `ElectronAuthenticator` e escopos necessários. 

Primeiro, abra *src/main.ts* e importe e a partir `ElectronAuthenticator` da parte superior da  `MsalElectronConfig` `@microsoft/mgt-electron-provider` página.

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
Em seguida, adicione essas linhas de código na função `createWindow()` para inicializar o EletrônicaAuthenticator, logo após onde `mainWindow` é declarado. Substitua `<your_client_id>` pela ID do cliente do registro do aplicativo.

```ts
const config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  mainWindow: mainWindow, //This is the BrowserWindow instance that requires authentication
  scopes: [
    'user.read',
        'user.read',
        'people.read',
        'user.readbasic.all',
        'contacts.read',
        'presence.read.all',
        'presence.read',
        'user.read.all',
        'calendars.read'
  ],
};
ElectronAuthenticator.initialize(config);
```

### <a name="set-nodeintegration-to-true"></a>Definir nodeIntegration como true
 
Em main.ts, onde a nova instância de BrowserWindow é criada, certifique-se de definir `nodeIntegration` como `true` em webPreferences. Se você ignorar essa etapa, poderá ter um ```Uncaught ReferenceError: require is not defined``` erro. Para manter isso simples, remova os scripts de pré-carregamento.

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a>Adicionar componentes à sua página HTML
 
Adicione algum conteúdo ao seu aplicativo. Agora você pode usar os componentes do kit de ferramentas do Microsoft Graph na página *index.html e* mostrar a agenda do usuário. Substitua o conteúdo da página *index.html* pelo seguinte.
 
 ```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Sample Electron-MGT App</title>
  </head>
  <body>
    <mgt-login></mgt-login>
    <mgt-agenda group-by-day></mgt-agenda>
    <script type="module" src="./dist/renderer.js"></script>
  </body>
</html>
 ```
 >**Observação:** Remova qualquer headers ou marcas de resposta de Política de Segurança de Conteúdo se você estiver copiando isso `meta` para um arquivo existente.
 
 ### <a name="bundle-your-app-using-webpack"></a>Agrupar seu aplicativo usando webpack
 
Antes de executar o aplicativo, você precisa agrupar seu código para garantir que todas as suas dependências modulares sejam incluídas na carga final. Se você já estiver codificando o código do aplicativo, ignore esta etapa.
 
 #### <a name="install-webpack"></a>Instalar webpack
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a>webpack.config.js
 
Crie um novo *arquivowebpack.config.js* na pasta raiz do seu projeto e colar a configuração a seguir.
 
 ```js
 const path = require('path');
 module.exports = [
  {
    mode: 'development',
    entry: './src/renderer.ts',
    target: 'electron-renderer',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'renderer.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  },
  {
    mode: 'development',
    entry: './src/main.ts',
    target: 'electron-main',
    module: {
      rules: [
        {
          test: /\.ts$/,
          include: [/src/],
          use: [{ loader: 'ts-loader' }]
        }
      ]
    },
    output: {
      path: __dirname + '/dist',
      filename: 'main.js'
    },
    resolve: {
      extensions: ['.ts', '.js'],
      modules: ['node_modules', path.resolve(__dirname + 'src')]
    }
  }
 ];

 ```
 
 Como você pode ver, o front-end (processo de renderização) e o back-end (processo principal), são agrupados separadamente. Isso ocorre porque, em Eletrônica, o processo de renderização é executado no contexto do navegador e o processo principal é executado no contexto do nó.
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a>Adicionar o script de webpacking em ```package.json```
 
 Adicione o seguinte em ```scripts``` em seu ```package.json``` .
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a>Executar seu aplicativo
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a>Adicionar recursos de cache de token ao seu aplicativo e habilitar logins silenciosos (avançados)

O Nó MSAL dá suporte a um cache na memória por padrão e fornece a interface ICachePlugin para executar a serialização de cache, mas não fornece uma maneira padrão de armazenar o cache de token em disco. Se você precisar de armazenamento de cache persistente para habilitar logins silenciosos ou cache entre plataformas, recomendamos usar a implementação padrão fornecida pelo Nó MSAL como [uma extensão](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions). Você pode importar esse plug-in e passar a instância do plug-in de cache ao inicializar `ElectronAuthenticator` .

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
Para obter mais detalhes sobre como implementar isso, consulte o [exemplo microsoft-authentication-library-for-js.](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js)

## <a name="next-steps"></a>Próximas etapas
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [o Microsoft Q&A](https://aka.ms/askgraph).
- Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).
    
