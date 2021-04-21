---
title: Usar o microsoft graph Toolkit com oTron
description: Começar a usar o microsoft graph Toolkit em um aplicativo Detron.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: b57315e3fcc44f94cc18d3f4a93826b00a5ce4b9
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920051"
---
# <a name="use-the-microsoft-graph-toolkit-with-electron"></a><span data-ttu-id="f14f3-103">Usar o microsoft graph Toolkit com oTron</span><span class="sxs-lookup"><span data-stu-id="f14f3-103">Use the Microsoft Graph Toolkit with Electron</span></span>

<span data-ttu-id="f14f3-104">Este artigo descreve o processo passo a passo de usar o microsoft graph Toolkit criar um aplicativo Detron e conectá-lo ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f14f3-104">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create an Electron app and connect it to Microsoft 365.</span></span> <span data-ttu-id="f14f3-105">Depois de concluir as etapas, você terá um aplicativo Detron que mostra os próximos compromissos do usuário atualmente inscrevado do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f14f3-105">After completing the steps, you'll have a Electron app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="create-an-electron-app"></a><span data-ttu-id="f14f3-106">Criar um aplicativo Detron</span><span class="sxs-lookup"><span data-stu-id="f14f3-106">Create an Electron app</span></span> 
<span data-ttu-id="f14f3-107">Crie um novo aplicativo Detron clonando [o repositório do tiposcript](https://github.com/electron/electron-quick-start-typescript) de início rápido do sistema.</span><span class="sxs-lookup"><span data-stu-id="f14f3-107">Create a new Electron app by cloning the [electron-quick-start-typescript](https://github.com/electron/electron-quick-start-typescript) repository.</span></span> <span data-ttu-id="f14f3-108">Isso criará um novo aplicativo Detron usando TypeScript, o que ajudará você a escrever um código mais robusto e a evitar erros de tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="f14f3-108">This will create a new Electron app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
git clone https://github.com/electron/electron-quick-start-typescript
```

<span data-ttu-id="f14f3-109">Altere o diretório de trabalho para o aplicativo recém-criado e instale todas as dependências.</span><span class="sxs-lookup"><span data-stu-id="f14f3-109">Change the working directory to the newly created app and install all dependencies.</span></span>

```cmd
cd electron-quick-start-typescript
npm install
```

<span data-ttu-id="f14f3-110">Instale o pacote "@microsoft/mgt-components" que contém todos os componentes web conectados ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f14f3-110">Install the '@microsoft/mgt-components' package that contains all the Microsoft Graph-connected web components.</span></span>

```cmd
npm i @microsoft/mgt-components
```

<span data-ttu-id="f14f3-111">Instale os `@microsoft/mgt-electron-provider` `@microsoft/mgt-element` pacotes e npm também.</span><span class="sxs-lookup"><span data-stu-id="f14f3-111">Install the `@microsoft/mgt-electron-provider` and `@microsoft/mgt-element` npm packages as well.</span></span> <span data-ttu-id="f14f3-112">Isso permitirá que você forneça autenticação para seu aplicativo usando o MSAL e use os componentes do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="f14f3-112">These will allow you to provide authentication for your app using MSAL and use the Microsoft Graph Toolkit components.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-electron-provider
```

<span data-ttu-id="f14f3-113">Confirme se você pode executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f14f3-113">Confirm that you can run the app.</span></span>

```cmd
npm start
```

## <a name="create-an-appclient-id"></a><span data-ttu-id="f14f3-114">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="f14f3-114">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-ad-to-get-a-client-id"></a><span data-ttu-id="f14f3-115">Adicionar novo registro de aplicativo no Azure AD para obter uma ID do cliente</span><span class="sxs-lookup"><span data-stu-id="f14f3-115">Add new application registration in Azure AD to get a client ID</span></span>

<span data-ttu-id="f14f3-116">Para criar um aplicativo no Azure Active Directory (Azure AD), você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e redirecionar o URI.</span><span class="sxs-lookup"><span data-stu-id="f14f3-116">To create an application in Azure Active Directory (Azure AD), you need to add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="f14f3-117">Para criar o aplicativo no Azure AD:</span><span class="sxs-lookup"><span data-stu-id="f14f3-117">To create the app in Azure AD:</span></span>

1. <span data-ttu-id="f14f3-118">Vá para o [portal do Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="f14f3-118">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="f14f3-119">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="f14f3-119">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="f14f3-120">No menu do Azure Active Directory, selecione **Registros de aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="f14f3-120">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="f14f3-121">No menu superior, selecione o **botão Novo registro.**</span><span class="sxs-lookup"><span data-stu-id="f14f3-121">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="f14f3-122">Insira o nome do seu aplicativo; por exemplo, `My Electron-App` .</span><span class="sxs-lookup"><span data-stu-id="f14f3-122">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="f14f3-123">Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório do **Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="f14f3-123">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="f14f3-124">No campo **Redirecionar URI,** no menu suspenso, selecione **Cliente público/nativo (área** de trabalho móvel &) e, no campo URL, digite `msal://redirect` .</span><span class="sxs-lookup"><span data-stu-id="f14f3-124">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="f14f3-125">Confirme as alterações selecionando o **botão Registrar.**</span><span class="sxs-lookup"><span data-stu-id="f14f3-125">Confirm changes by selecting the **Register** button.</span></span>
1. <span data-ttu-id="f14f3-126">Vá para o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f14f3-126">Go to your application registration.</span></span>
1. <span data-ttu-id="f14f3-127">Verifique se você está na página **Visão** Geral.</span><span class="sxs-lookup"><span data-stu-id="f14f3-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="f14f3-128">Na seção **Essentials,** copie o valor da propriedade **Application (client).**</span><span class="sxs-lookup"><span data-stu-id="f14f3-128">From the **Essentials** section, copy the value of the **Application (client) ID** property.</span></span>

## <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="f14f3-129">Configurar o provedor de autenticação Toolkit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f14f3-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

### <a name="initializing-electronprovider-in-your-renderer-process"></a><span data-ttu-id="f14f3-130">Inicializando oTronProvider no processo de renderização</span><span class="sxs-lookup"><span data-stu-id="f14f3-130">Initializing ElectronProvider in your renderer process</span></span>

<span data-ttu-id="f14f3-131">O responsável por se comunicar com (no processo principal) para solicitar tokens de acesso e receber informações sobre o estado assinado que é necessário para que os `ElectronProvider` `ElectronAuthenticator` componentes mgt funcionem.</span><span class="sxs-lookup"><span data-stu-id="f14f3-131">The `ElectronProvider` is responsible for communicating with `ElectronAuthenticator` (in the main process) to request access tokens and receive information regarding signed in state that is required for the mgt components to work.</span></span> 

<span data-ttu-id="f14f3-132">Para inicializar o arquivo , adicione o código a `ElectronProvider` seguir ao *arquivo src/renderer.ts.*</span><span class="sxs-lookup"><span data-stu-id="f14f3-132">To initialize the `ElectronProvider`, add the following code to the *src/renderer.ts* file.</span></span>
```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
// import the mgt components so we can use them in our html
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-your-main-process"></a><span data-ttu-id="f14f3-133">Inicializando o EletrônicaAuthenticator em seu processo principal</span><span class="sxs-lookup"><span data-stu-id="f14f3-133">Initializing ElectronAuthenticator in your main process</span></span>

<span data-ttu-id="f14f3-134">O é responsável por configurar as variáveis de configuração para autenticação `ElectronAuthenticator` MSAL, adquirir tokens de acesso e se comunicar com `ElectronProvider` o .</span><span class="sxs-lookup"><span data-stu-id="f14f3-134">The `ElectronAuthenticator` is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with the `ElectronProvider`.</span></span> <span data-ttu-id="f14f3-135">Inicializar o no processo principal e configurar as variáveis de configuração, como iD do cliente `ElectronAuthenticator` e escopos necessários.</span><span class="sxs-lookup"><span data-stu-id="f14f3-135">Initialize the `ElectronAuthenticator` in the main process and set up the configuration variables such as client ID and required scopes.</span></span> 

<span data-ttu-id="f14f3-136">Primeiro, abra *src/main.ts* e importe e a partir `ElectronAuthenticator` da parte superior da  `MsalElectronConfig` `@microsoft/mgt-electron-provider` página.</span><span class="sxs-lookup"><span data-stu-id="f14f3-136">First, open *src/main.ts* and import `ElectronAuthenticator` and  `MsalElectronConfig` from `@microsoft/mgt-electron-provider` at the top of the page.</span></span>

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 
```
<span data-ttu-id="f14f3-137">Em seguida, adicione essas linhas de código na função `createWindow()` para inicializar o EletrônicaAuthenticator, logo após onde `mainWindow` é declarado.</span><span class="sxs-lookup"><span data-stu-id="f14f3-137">Next, add these lines of code in the `createWindow()` function to initialize the ElectronAuthenticator, right after where `mainWindow` is declared.</span></span> <span data-ttu-id="f14f3-138">Substitua `<your_client_id>` pela ID do cliente do registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f14f3-138">Replace `<your_client_id>` with the client ID from your app registration.</span></span>

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

### <a name="set-nodeintegration-to-true"></a><span data-ttu-id="f14f3-139">Definir nodeIntegration como true</span><span class="sxs-lookup"><span data-stu-id="f14f3-139">Set nodeIntegration to true</span></span>
 
<span data-ttu-id="f14f3-140">Em main.ts, onde a nova instância de BrowserWindow é criada, certifique-se de definir `nodeIntegration` como `true` em webPreferences.</span><span class="sxs-lookup"><span data-stu-id="f14f3-140">In main.ts, where the new instance of BrowserWindow is created, make sure that you set `nodeIntegration` to `true` under webPreferences.</span></span> <span data-ttu-id="f14f3-141">Se você ignorar essa etapa, poderá ter um ```Uncaught ReferenceError: require is not defined``` erro.</span><span class="sxs-lookup"><span data-stu-id="f14f3-141">If you skip this step, you might run into a ```Uncaught ReferenceError: require is not defined``` error.</span></span> <span data-ttu-id="f14f3-142">Para manter isso simples, remova os scripts de pré-carregamento.</span><span class="sxs-lookup"><span data-stu-id="f14f3-142">To keep this simple, remove any preloading scripts.</span></span>

```ts
const mainWindow = new BrowserWindow({
  height: 600,
  webPreferences: {
    nodeIntegration: true //Set this to true
  },
  width: 800
});
```
 
### <a name="add-components-to-your-html-page"></a><span data-ttu-id="f14f3-143">Adicionar componentes à sua página HTML</span><span class="sxs-lookup"><span data-stu-id="f14f3-143">Add components to your HTML page</span></span>
 
<span data-ttu-id="f14f3-144">Adicione algum conteúdo ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f14f3-144">Add some content to your app.</span></span> <span data-ttu-id="f14f3-145">Agora você pode usar os componentes do kit de ferramentas do Microsoft Graph na página *index.html e* mostrar a agenda do usuário.</span><span class="sxs-lookup"><span data-stu-id="f14f3-145">You can now use the Microsoft Graph toolkit components in your *index.html* page and show the user's agenda.</span></span> <span data-ttu-id="f14f3-146">Substitua o conteúdo da página *index.html* pelo seguinte.</span><span class="sxs-lookup"><span data-stu-id="f14f3-146">Replace the content of the *index.html* page with the following.</span></span>
 
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
 ><span data-ttu-id="f14f3-147">**Observação:** Remova qualquer headers ou marcas de resposta de Política de Segurança de Conteúdo se você estiver copiando isso `meta` para um arquivo existente.</span><span class="sxs-lookup"><span data-stu-id="f14f3-147">**Note:** Remove any Content-Security-Policy response headers or `meta` tags if you are copying this onto an existing file.</span></span>
 
 ### <a name="bundle-your-app-using-webpack"></a><span data-ttu-id="f14f3-148">Agrupar seu aplicativo usando webpack</span><span class="sxs-lookup"><span data-stu-id="f14f3-148">Bundle your app using webpack</span></span>
 
<span data-ttu-id="f14f3-149">Antes de executar o aplicativo, você precisa agrupar seu código para garantir que todas as suas dependências modulares sejam incluídas na carga final.</span><span class="sxs-lookup"><span data-stu-id="f14f3-149">Before you can run the app, you  need to bundle your code to ensure that all your modular dependencies are included in the final payload.</span></span> <span data-ttu-id="f14f3-150">Se você já estiver codificando o código do aplicativo, ignore esta etapa.</span><span class="sxs-lookup"><span data-stu-id="f14f3-150">If you are already bundling your app code, you can skip this step.</span></span>
 
 #### <a name="install-webpack"></a><span data-ttu-id="f14f3-151">Instalar webpack</span><span class="sxs-lookup"><span data-stu-id="f14f3-151">Install webpack</span></span>
 
 ```cmd 
 npm install webpack webpack-cli ts-loader --save-dev
 ```
 
 #### <a name="webpackconfigjs"></a><span data-ttu-id="f14f3-152">webpack.config.js</span><span class="sxs-lookup"><span data-stu-id="f14f3-152">webpack.config.js</span></span>
 
<span data-ttu-id="f14f3-153">Crie um novo *arquivowebpack.config.js* na pasta raiz do seu projeto e colar a configuração a seguir.</span><span class="sxs-lookup"><span data-stu-id="f14f3-153">Create a new *webpack.config.js* file in the root folder of your project, and paste the following configuration.</span></span>
 
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
 
 <span data-ttu-id="f14f3-154">Como você pode ver, o front-end (processo de renderização) e o back-end (processo principal), são agrupados separadamente.</span><span class="sxs-lookup"><span data-stu-id="f14f3-154">As you can see, the front end (renderer process) and the back-end (main process), are bundled separately.</span></span> <span data-ttu-id="f14f3-155">Isso ocorre porque, em Eletrônica, o processo de renderização é executado no contexto do navegador e o processo principal é executado no contexto do nó.</span><span class="sxs-lookup"><span data-stu-id="f14f3-155">This is because in Electron, the renderer process runs in the browser context and the main process runs in the node context.</span></span>
 
 #### <a name="add-the-webpacking-script-in-packagejson"></a><span data-ttu-id="f14f3-156">Adicionar o script de webpacking em ```package.json```</span><span class="sxs-lookup"><span data-stu-id="f14f3-156">Add the webpacking script in ```package.json```</span></span>
 
 <span data-ttu-id="f14f3-157">Adicione o seguinte em ```scripts``` em seu ```package.json``` .</span><span class="sxs-lookup"><span data-stu-id="f14f3-157">Add the following under ```scripts``` in your ```package.json```.</span></span>
 
 ```json
"scripts": {
   "webpack": "webpack",
   "start": "npm run webpack && electron dist/main.js"
 }                
 ```
 
 #### <a name="run-your-app"></a><span data-ttu-id="f14f3-158">Executar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="f14f3-158">Run your app</span></span>
 
 ```cmd
 npm start
 ```

### <a name="add-token-caching-capabilities-to-your-app-and-enable-silent-sign-ins-advanced"></a><span data-ttu-id="f14f3-159">Adicionar recursos de cache de token ao seu aplicativo e habilitar logins silenciosos (avançados)</span><span class="sxs-lookup"><span data-stu-id="f14f3-159">Add token caching capabilities to your app and enable silent sign ins (advanced)</span></span>

<span data-ttu-id="f14f3-160">O Nó MSAL dá suporte a um cache na memória por padrão e fornece a interface ICachePlugin para executar a serialização de cache, mas não fornece uma maneira padrão de armazenar o cache de token em disco.</span><span class="sxs-lookup"><span data-stu-id="f14f3-160">MSAL Node supports an in-memory cache by default and provides the ICachePlugin interface to perform cache serialization, but does not provide a default way of storing the token cache to disk.</span></span> <span data-ttu-id="f14f3-161">Se você precisar de armazenamento de cache persistente para habilitar logins silenciosos ou cache entre plataformas, recomendamos usar a implementação padrão fornecida pelo Nó MSAL como [uma extensão](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span><span class="sxs-lookup"><span data-stu-id="f14f3-161">If you need persistent cache storage to enable silent sign ins or cross-platform caching, we recommend using the default implementation provided by MSAL Node as an [extension](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="f14f3-162">Você pode importar esse plug-in e passar a instância do plug-in de cache ao inicializar `ElectronAuthenticator` .</span><span class="sxs-lookup"><span data-stu-id="f14f3-162">You can import this plugin, and pass the instance of the cache plugin while initializing `ElectronAuthenticator`.</span></span>

```ts
let config: MsalElectronConfig = {
  ...
  cachePlugin: new PersistenceCachePlugin(filePersistence) //filePersistence is the instance of type IPersistence that you will need to create
};
```
<span data-ttu-id="f14f3-163">Para obter mais detalhes sobre como implementar isso, consulte o [exemplo microsoft-authentication-library-for-js.](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js)</span><span class="sxs-lookup"><span data-stu-id="f14f3-163">For more details about how to implement this, see the [microsoft-authentication-library-for-js](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/dev/extensions/samples/msal-node-extensions/index.js) sample.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f14f3-164">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="f14f3-164">Next Steps</span></span>
- <span data-ttu-id="f14f3-165">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="f14f3-165">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="f14f3-166">Faça uma pergunta sobre [o Microsoft Q&A](/answers/products/m365#microsoft-graph).</span><span class="sxs-lookup"><span data-stu-id="f14f3-166">Ask a question on [Microsoft Q&A](/answers/products/m365#microsoft-graph).</span></span>
- <span data-ttu-id="f14f3-167">Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="f14f3-167">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
