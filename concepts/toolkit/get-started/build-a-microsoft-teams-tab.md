---
title: Criar uma guia do Microsoft Teams com o Microsoft Graph Toolkit
description: Começar a criar uma guia do Microsoft Teams usando o microsoft graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 915bbe562fec9ef0bcbd5ae6d67d8497ea7e72eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963271"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="d08ad-103">Criar uma guia do Microsoft Teams com o Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d08ad-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d08ad-104">Este tópico aborda como começar a usar o microsoft graph Toolkit em uma solução do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d08ad-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="d08ad-105">Começar envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="d08ad-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="d08ad-106">Crie um novo aplicativo do Teams com uma guia personalizada.</span><span class="sxs-lookup"><span data-stu-id="d08ad-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="d08ad-107">Adicione o microsoft graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="d08ad-107">Add the Microsoft Graph Toolkit.</span></span>
3. <span data-ttu-id="d08ad-108">Inicializar o provedor do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d08ad-108">Initialize the Microsoft Teams provider.</span></span>
4. <span data-ttu-id="d08ad-109">Crie a página pop-up de auth.</span><span class="sxs-lookup"><span data-stu-id="d08ad-109">Create the auth popup page.</span></span>
5. <span data-ttu-id="d08ad-110">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="d08ad-110">Add components.</span></span>
6. <span data-ttu-id="d08ad-111">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d08ad-111">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="d08ad-112">Criar um novo aplicativo do Teams com uma guia personalizada</span><span class="sxs-lookup"><span data-stu-id="d08ad-112">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="d08ad-113">A maneira mais fácil de criar um novo aplicativo do Teams é usar a extensão Toolkit [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) para Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="d08ad-113">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="d08ad-114">Siga as instruções para [configurar um novo projeto do Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)</span><span class="sxs-lookup"><span data-stu-id="d08ad-114">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="d08ad-115">Quando você chegar à tela **Adicionar recursos,** selecione **Guia** e, em seguida, **guia Pessoal.**</span><span class="sxs-lookup"><span data-stu-id="d08ad-115">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="d08ad-116">Adicionar o microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d08ad-116">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d08ad-117">Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="d08ad-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="d08ad-118">Para usar o Toolkit, você também precisará do [SDK do Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)</span><span class="sxs-lookup"><span data-stu-id="d08ad-118">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="d08ad-119">Usar por meio do mgt-loader</span><span class="sxs-lookup"><span data-stu-id="d08ad-119">Use via mgt-loader</span></span>
<span data-ttu-id="d08ad-120">Para usar o Toolkit e o SDK do Teams por meio dos carregadores, adicione as seguintes referências dentro `<head>` do `public/index.html` arquivo:</span><span class="sxs-lookup"><span data-stu-id="d08ad-120">To use the Toolkit and the Teams SDK via the loaders, add the following references inside the `<head>` of the `public/index.html` file:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="d08ad-121">Usar por npm (módulos ES6)</span><span class="sxs-lookup"><span data-stu-id="d08ad-121">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="d08ad-122">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d08ad-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="d08ad-123">Para usar os módulos ES6, adicione os pacotes npm para o Toolkit e o SDK do Microsoft Teams ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="d08ad-123">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="d08ad-124">Inicializar o provedor do Teams</span><span class="sxs-lookup"><span data-stu-id="d08ad-124">Initialize the Teams provider</span></span>

<span data-ttu-id="d08ad-125">Os provedores Toolkit Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="d08ad-125">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="d08ad-126">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d08ad-126">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="d08ad-127">O [provedor do Teams](../providers/teams.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK do Teams para autenticar o usuário.</span><span class="sxs-lookup"><span data-stu-id="d08ad-127">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="d08ad-128">Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d08ad-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="d08ad-129">Inicializar em HTML</span><span class="sxs-lookup"><span data-stu-id="d08ad-129">Initialize in HTML</span></span>

<span data-ttu-id="d08ad-130">In `public/index.html` , add the Teams provider into the , as `<body>` shown.</span><span class="sxs-lookup"><span data-stu-id="d08ad-130">In `public/index.html`, add the Teams provider into the `<body>`, as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="d08ad-131">Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d08ad-131">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span> 

### <a name="initialize-in-javascript"></a><span data-ttu-id="d08ad-132">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="d08ad-132">Initialize in JavaScript</span></span>

<span data-ttu-id="d08ad-133">Para inicializar o provedor em seu código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto.</span><span class="sxs-lookup"><span data-stu-id="d08ad-133">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="d08ad-134">Importe o Provedor do Teams e inicialize o provedor.</span><span class="sxs-lookup"><span data-stu-id="d08ad-134">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="d08ad-135">Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d08ad-135">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="d08ad-136">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="d08ad-136">Creating an app/client ID</span></span>

<span data-ttu-id="d08ad-137">Para obter uma ID do cliente, você precisa registrar um aplicativo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d08ad-137">To get a client ID, you need to register an Azure Active Directory application.</span></span> <span data-ttu-id="d08ad-138">Siga as etapas no [artigo Criar um aplicativo do Azure Active Directory.](./add-aad-app-registration.md)</span><span class="sxs-lookup"><span data-stu-id="d08ad-138">Follow the steps in the [Create an Azure Active Directory app](./add-aad-app-registration.md) article.</span></span>

<span data-ttu-id="d08ad-139">Certifique-se de definir o **URI de** redirecionamento no registro do aplicativo para apontar para sua `auth.html` página.</span><span class="sxs-lookup"><span data-stu-id="d08ad-139">Make sure to set the **redirect URI** in your app registration to point to your `auth.html` page.</span></span> <span data-ttu-id="d08ad-140">Por exemplo, se você estiver executando seu aplicativo `localhost:3000` em , de definir o URI de redirecionamento como `https://localhost:3000/auth.html` .</span><span class="sxs-lookup"><span data-stu-id="d08ad-140">For example, if you are running your app on `localhost:3000`, set the redirect URI to `https://localhost:3000/auth.html`.</span></span>

><span data-ttu-id="d08ad-141">**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="d08ad-141">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="d08ad-142">Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="d08ad-142">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="d08ad-143">Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="d08ad-143">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="d08ad-144">Criar a página pop-up de auth</span><span class="sxs-lookup"><span data-stu-id="d08ad-144">Create the auth popup page</span></span>

<span data-ttu-id="d08ad-145">Para permitir que os usuários entre, você precisa fornecer uma URL que o aplicativo do Teams abrirá em um pop-up para seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="d08ad-145">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="d08ad-146">A URL precisa estar em seu domínio, e tudo o que essa página precisa fazer é chamar o `TeamsProvider.handleAuth()` método.</span><span class="sxs-lookup"><span data-stu-id="d08ad-146">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="d08ad-147">Você pode fazer isso adicionando um novo arquivo na pasta (que deve estar no mesmo nível que ) e adicionando `auth.html` `public` o seguinte `index.html` código:</span><span class="sxs-lookup"><span data-stu-id="d08ad-147">You can do this by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
```

## <a name="add-components"></a><span data-ttu-id="d08ad-148">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="d08ad-148">Add components</span></span>

<span data-ttu-id="d08ad-149">Agora, você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à guia.</span><span class="sxs-lookup"><span data-stu-id="d08ad-149">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="d08ad-150">Você pode adicionar componentes ao HTML como normalmente faria.</span><span class="sxs-lookup"><span data-stu-id="d08ad-150">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="d08ad-151">Por exemplo, para adicionar o componente Logon, adicione o código abaixo ao corpo do `index.html` seu :</span><span class="sxs-lookup"><span data-stu-id="d08ad-151">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="d08ad-152">Ou você pode adicionar os componentes no JSX ao componente Tab.</span><span class="sxs-lookup"><span data-stu-id="d08ad-152">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="d08ad-153">Recomendamos o uso `mgt-react` da biblioteca se você criou seu aplicativo do Teams usando a extensão microsoft teams Toolkit extensão.</span><span class="sxs-lookup"><span data-stu-id="d08ad-153">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="d08ad-154">Para saber mais, consulte [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="d08ad-154">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="d08ad-155">Primeiro, instale `mgt-react` :</span><span class="sxs-lookup"><span data-stu-id="d08ad-155">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="d08ad-156">Localize `src/components/Tab.js` o arquivo e importe os componentes que você deseja usar na `mgt-react` biblioteca.</span><span class="sxs-lookup"><span data-stu-id="d08ad-156">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="d08ad-157">Por exemplo, para adicionar o `Login` uso do componente:</span><span class="sxs-lookup"><span data-stu-id="d08ad-157">For example, to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="d08ad-158">Em seguida, adicione o componente à `return()` instrução do `render()` método de `Tab` :</span><span class="sxs-lookup"><span data-stu-id="d08ad-158">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="d08ad-159">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="d08ad-159">Test your application</span></span>

<span data-ttu-id="d08ad-160">Crie e execute seu aplicativo usando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d08ad-160">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="d08ad-161">Para testar seu aplicativo, você pode instalar seu aplicativo no Teams por meio do Teams Toolkit Extension.</span><span class="sxs-lookup"><span data-stu-id="d08ad-161">To test your application, you can install your app to Teams via the Teams Toolkit Extension.</span></span> <span data-ttu-id="d08ad-162">Abra o Teams Toolkit Extension e **clique em Abrir o Microsoft Teams Toolkit**.</span><span class="sxs-lookup"><span data-stu-id="d08ad-162">Open the Teams Toolkit Extension and click **Open Microsoft Teams Toolkit**.</span></span> <span data-ttu-id="d08ad-163">Clique **em App Studio** no menu esquerdo, role para baixo e selecione Testar e **Distribuir**, em **seguida, Instalar**.</span><span class="sxs-lookup"><span data-stu-id="d08ad-163">Click **App Studio** in the left menu, scroll down and select **Test and Distribute**, then **Install**.</span></span> <span data-ttu-id="d08ad-164">O Teams abrirá no navegador e você será redirecionado para a guia criada.</span><span class="sxs-lookup"><span data-stu-id="d08ad-164">Teams will open in your browser, and you will be redirected to the tab you created.</span></span> <span data-ttu-id="d08ad-165">Você deve ser capaz de ver o componente de Logon e usá-lo para entrar no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d08ad-165">You should be able to see the Login component and use it to sign in to your application.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d08ad-166">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d08ad-166">Next Steps</span></span>
- <span data-ttu-id="d08ad-167">Confira este tutorial passo a passo sobre [como criar uma guia do Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)</span><span class="sxs-lookup"><span data-stu-id="d08ad-167">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="d08ad-168">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="d08ad-168">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="d08ad-169">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="d08ad-169">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="d08ad-170">Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="d08ad-170">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
