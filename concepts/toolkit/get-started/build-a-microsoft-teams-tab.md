---
title: Criar uma guia do Microsoft Teams com o Kit de Ferramentas do Microsoft Graph
description: Começar a criar uma guia do Microsoft Teams usando o Kit de Ferramentas do Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 96a820fa26697d360128b86ea8ba7cbd4d3c1cd8
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072349"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="13937-103">Criar uma guia do Microsoft Teams com o Kit de Ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13937-103">Build a Microsoft Teams tab with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="13937-104">Este tópico aborda como começar a usar o Microsoft Graph Toolkit em uma solução do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13937-104">This topic covers how to get started using the Microsoft Graph Toolkit in a Microsoft Teams solution.</span></span> <span data-ttu-id="13937-105">A iniciação envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="13937-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="13937-106">Crie um novo aplicativo teams com uma guia personalizada.</span><span class="sxs-lookup"><span data-stu-id="13937-106">Create a new Teams application with a custom tab.</span></span>
2. <span data-ttu-id="13937-107">Configurar o ngrok e criar um túnel.</span><span class="sxs-lookup"><span data-stu-id="13937-107">Set up ngrok and create a tunnel.</span></span>
3. <span data-ttu-id="13937-108">Adicione o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="13937-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="13937-109">Inicialize o provedor do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13937-109">Initialize the Microsoft Teams provider.</span></span>
5. <span data-ttu-id="13937-110">Crie a página pop-up de auth.</span><span class="sxs-lookup"><span data-stu-id="13937-110">Create the auth popup page.</span></span>
6. <span data-ttu-id="13937-111">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="13937-111">Add components.</span></span>
7. <span data-ttu-id="13937-112">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13937-112">Test your app.</span></span>

## <a name="create-a-new-teams-application-with-a-custom-tab"></a><span data-ttu-id="13937-113">Criar um novo aplicativo teams com uma guia personalizada</span><span class="sxs-lookup"><span data-stu-id="13937-113">Create a new Teams application with a custom tab</span></span>

<span data-ttu-id="13937-114">A maneira mais fácil de criar um novo aplicativo teams é usar a extensão do Kit de [Ferramentas do Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) para o Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="13937-114">The easiest way to create a new Teams app is to use the [Microsoft Teams Toolkit extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) for Visual Studio Code.</span></span> <span data-ttu-id="13937-115">Siga as instruções para [configurar um novo projeto do Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project)</span><span class="sxs-lookup"><span data-stu-id="13937-115">Follow the instructions to [set up a new Teams project](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project).</span></span> <span data-ttu-id="13937-116">Quando você chegar à tela **Adicionar recursos,** selecione **Tab** e, em seguida, **a guia Pessoal.**</span><span class="sxs-lookup"><span data-stu-id="13937-116">When you get to the **Add capabilities** screen, select **Tab**, and then **Personal tab**.</span></span>

## <a name="set-up-ngrok-and-create-a-tunnel"></a><span data-ttu-id="13937-117">Configurar o ngrok e criar um túnel</span><span class="sxs-lookup"><span data-stu-id="13937-117">Set up ngrok and create a tunnel</span></span>

<span data-ttu-id="13937-118">Para testar seu aplicativo posteriormente, você precisará hospedar seu aplicativo em uma URL voltada para o público usando HTTPS.</span><span class="sxs-lookup"><span data-stu-id="13937-118">In order to test your application later, you will need to host your application over a public-facing URL using HTTPS.</span></span> <span data-ttu-id="13937-119">Instale [o ngrok](https://ngrok.com/download) e crie um túnel da Internet para o localhost:3000 com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="13937-119">Install [ngrok](https://ngrok.com/download) and create a tunnel from the Internet to localhost:3000 with the following command:</span></span>

```bash
ngrok http 3000
```
<span data-ttu-id="13937-120">No diretório do projeto, localize `.publish\Development.env` o arquivo e substitua o valor pela URL do `baseUrl0` ngrok.</span><span class="sxs-lookup"><span data-stu-id="13937-120">In your project directory, locate the `.publish\Development.env` file and replace the value for `baseUrl0` with your ngrok URL.</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="13937-121">Adicionar o Kit de Ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13937-121">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="13937-122">Você pode usar o Microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="13937-122">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span> <span data-ttu-id="13937-123">Para usar o Kit de Ferramentas, você também precisará do [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13937-123">To use the Toolkit, you will also need the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="13937-124">Usar via mgt-loader</span><span class="sxs-lookup"><span data-stu-id="13937-124">Use via mgt-loader</span></span>
<span data-ttu-id="13937-125">Para usar o Kit de Ferramentas e o SDK do Teams por meio dos carregadores, adicione as seguintes referências `public/index.html` a:</span><span class="sxs-lookup"><span data-stu-id="13937-125">To use the Toolkit and the Teams SDK via the loaders, add the following references to `public/index.html`:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="13937-126">Usar via npm (módulos ES6)</span><span class="sxs-lookup"><span data-stu-id="13937-126">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="13937-127">Usar o Kit de Ferramentas por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá agrupar apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13937-127">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="13937-128">Para usar os módulos ES6, adicione os pacotes npm para o Kit de Ferramentas e o SDK do Microsoft Teams ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="13937-128">To use the ES6 modules, add the npm packages for both the Toolkit and the Microsoft Teams SDK to your project:</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a><span data-ttu-id="13937-129">Inicializar o provedor do Teams</span><span class="sxs-lookup"><span data-stu-id="13937-129">Initialize the Teams provider</span></span>

<span data-ttu-id="13937-130">Os provedores do Microsoft Graph Toolkit permitem autenticação e acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="13937-130">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="13937-131">Para saber mais, consulte [Usando os provedores.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="13937-131">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="13937-132">O [provedor do Teams](../providers/teams.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK do Teams para autenticar o usuário.</span><span class="sxs-lookup"><span data-stu-id="13937-132">The [Teams provider](../providers/teams.md) handles all of the logic and interactions that need to be implemented with the Teams SDK to authenticate the user.</span></span>

<span data-ttu-id="13937-133">Você pode optar por inicializar o provedor no código HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="13937-133">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-html"></a><span data-ttu-id="13937-134">Inicializar em HTML</span><span class="sxs-lookup"><span data-stu-id="13937-134">Initialize in HTML</span></span>

<span data-ttu-id="13937-135">Em `public/index.html` , adicione o provedor do Teams conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="13937-135">In `public/index.html`, add the Teams provider as shown.</span></span>

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

<span data-ttu-id="13937-136">Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo e pela `<YOUR_NGROK_URL>` URL ngrok que você criou.</span><span class="sxs-lookup"><span data-stu-id="13937-136">Replace `<YOUR_CLIENT_ID>` with the client ID for your application and `<YOUR_NGROK_URL>` with the ngrok URL you created.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="13937-137">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="13937-137">Initialize in JavaScript</span></span>

<span data-ttu-id="13937-138">Para inicializar o provedor no código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto.</span><span class="sxs-lookup"><span data-stu-id="13937-138">To initialize the provider in your JavaScript code, Locate the `src/components/App.js` file in your project directory.</span></span> <span data-ttu-id="13937-139">Importe o Provedor do Teams e inicialize o provedor.</span><span class="sxs-lookup"><span data-stu-id="13937-139">Import the Teams Provider and initialize the provider.</span></span>

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
<span data-ttu-id="13937-140">Substitua `<YOUR_CLIENT_ID>` pela ID do cliente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13937-140">Replace `<YOUR_CLIENT_ID>` with the client ID for your application.</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="13937-141">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="13937-141">Creating an app/client ID</span></span>
<span data-ttu-id="13937-142">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../../auth-register-app-v2.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13937-142">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> <span data-ttu-id="13937-143">Certifique-se de adicionar sua URL ngrok com o caminho completo para a página pop-up de autenticação para seus URIs de redirecionamento (por exemplo, `https://<YOUR_NGROK_URL>/auth.html` ).</span><span class="sxs-lookup"><span data-stu-id="13937-143">Make sure to add your ngrok URL with the full path to the auth popup page to your redirect URIs (for example, `https://<YOUR_NGROK_URL>/auth.html`).</span></span>
><span data-ttu-id="13937-144">**Observação:** A MSAL só dá suporte ao Fluxo Implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="13937-144">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="13937-145">Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="13937-145">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="13937-146">Em **Autenticação,** encontre a **seção concessão implícita** e marque as caixas de seleção para **tokens do Access** e **tokens de ID.**</span><span class="sxs-lookup"><span data-stu-id="13937-146">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="create-the-auth-popup-page"></a><span data-ttu-id="13937-147">Criar a página pop-up de auth</span><span class="sxs-lookup"><span data-stu-id="13937-147">Create the auth popup page</span></span>

<span data-ttu-id="13937-148">Para permitir que os usuários se inscrevam, você precisa fornecer uma URL que o aplicativo teams abrirá em um pop-up para seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="13937-148">In order to allow users to sign in, you need to provide a URL that the Teams app will open in a popup to follow the authentication flow.</span></span> <span data-ttu-id="13937-149">A URL precisa estar em seu domínio, e tudo o que essa página precisa fazer é chamar o `TeamsProvider.handleAuth()` método.</span><span class="sxs-lookup"><span data-stu-id="13937-149">The URL needs to be in your domain, and all this page needs to do is call the `TeamsProvider.handleAuth()` method.</span></span>

<span data-ttu-id="13937-150">Você pode fazer isso em seu HTML adicionando um novo arquivo na pasta (que deve estar no mesmo nível que ) e adicionando `auth.html` `public` o seguinte `index.html` código:</span><span class="sxs-lookup"><span data-stu-id="13937-150">You can do this in your HTML by adding a new `auth.html` file in the `public` folder (which should be at the same level as `index.html`) and adding the following code:</span></span> 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a><span data-ttu-id="13937-151">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="13937-151">Add components</span></span>

<span data-ttu-id="13937-152">Agora você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à guia.</span><span class="sxs-lookup"><span data-stu-id="13937-152">Now, you're ready to add any of the Microsoft Graph Toolkit components to your tab.</span></span> 

<span data-ttu-id="13937-153">Você pode adicionar componentes ao HTML como faria normalmente.</span><span class="sxs-lookup"><span data-stu-id="13937-153">You can add components to your HTML as you normally would.</span></span> <span data-ttu-id="13937-154">Por exemplo, para adicionar o componente de logon, adicione o código a seguir ao corpo do `index.html` seu:</span><span class="sxs-lookup"><span data-stu-id="13937-154">For example, to add the Login component add the below code to the body of your `index.html`:</span></span>

```html
<mgt-login></mgt-login>
```

<span data-ttu-id="13937-155">Ou você pode adicionar os componentes no JSX ao componente Tab.</span><span class="sxs-lookup"><span data-stu-id="13937-155">Or, you can add the components in JSX to the Tab component.</span></span> <span data-ttu-id="13937-156">Recomendamos usar a biblioteca se você tiver criado seu aplicativo Teams usando a extensão do Kit de `mgt-react` Ferramentas do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="13937-156">We recommend using the `mgt-react` library if you created your Teams app using the Microsoft Teams Toolkit extension.</span></span> <span data-ttu-id="13937-157">Para saber mais, confira [Como usar o Kit de Ferramentas do Microsoft Graph com o React](./use-toolkit-with-react.md)</span><span class="sxs-lookup"><span data-stu-id="13937-157">To learn more, see [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)</span></span>

<span data-ttu-id="13937-158">Primeiro, `mgt-react` instale:</span><span class="sxs-lookup"><span data-stu-id="13937-158">First, install `mgt-react`:</span></span>

```bash
npm install @microsoft/mgt-react
```

<span data-ttu-id="13937-159">Localize `src/components/Tab.js` o arquivo e importe os componentes que você deseja usar da `mgt-react` biblioteca.</span><span class="sxs-lookup"><span data-stu-id="13937-159">Locate the `src/components/Tab.js` file and import the components you want to use from the `mgt-react` library.</span></span> <span data-ttu-id="13937-160">Por exemplo, para adicionar o `Login` uso do componente:</span><span class="sxs-lookup"><span data-stu-id="13937-160">For example, to add the `Login` component use:</span></span>

```js
import { Login } from "@microsoft/mgt-react"
```

<span data-ttu-id="13937-161">Em seguida, adicione o componente à `return()` instrução do `render()` método `Tab` de:</span><span class="sxs-lookup"><span data-stu-id="13937-161">Then, add the the component to the `return()` statement of the `render()` method of `Tab`:</span></span>

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a><span data-ttu-id="13937-162">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="13937-162">Test your application</span></span>

<span data-ttu-id="13937-163">Crie e execute seu aplicativo usando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="13937-163">Build and run your application using the following commands:</span></span>
```bash
npm install
npm start
```

<span data-ttu-id="13937-164">Para testar seu aplicativo, você precisa carregar seu aplicativo para o Teams.</span><span class="sxs-lookup"><span data-stu-id="13937-164">To test your application, you need to upload your application to Teams.</span></span> <span data-ttu-id="13937-165">Abra o cliente do Microsoft Teams, selecione **o...** no menu à esquerda e vá para **o App Studio.**</span><span class="sxs-lookup"><span data-stu-id="13937-165">Open the Microsoft Teams client, select the **...** on the left-hand menu and go to **App Studio**.</span></span> <span data-ttu-id="13937-166">Clique na **guia Editor de** Manifesto e selecione Importar um aplicativo **existente.**</span><span class="sxs-lookup"><span data-stu-id="13937-166">Click the **Manifest Editor** tab and select **Import an existing app**.</span></span>

<span data-ttu-id="13937-167">Localize o diretório do projeto **e carregue oDevelopment.zip** arquivo dentro da pasta **.publish.**</span><span class="sxs-lookup"><span data-stu-id="13937-167">Locate your project directory and upload the **Development.zip** file inside of the **.publish** folder.</span></span>

<span data-ttu-id="13937-168">Depois que seu aplicativo tiver carregado, role para baixo no menu à esquerda e selecione **Testar e Distribuir.**</span><span class="sxs-lookup"><span data-stu-id="13937-168">After your app has loaded, scroll down on the left menu and select **Test and Distribute**.</span></span> <span data-ttu-id="13937-169">Clique no **botão Instalar** e clique em **Adicionar.**</span><span class="sxs-lookup"><span data-stu-id="13937-169">Click the **Install** button and then click **Add**.</span></span> <span data-ttu-id="13937-170">Você será redirecionado para a guia que você criou.</span><span class="sxs-lookup"><span data-stu-id="13937-170">You will be redirected to the tab you created.</span></span>

## <a name="next-steps"></a><span data-ttu-id="13937-171">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="13937-171">Next Steps</span></span>
- <span data-ttu-id="13937-172">Confira este tutorial passo a passo sobre como [criar uma guia do Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)</span><span class="sxs-lookup"><span data-stu-id="13937-172">Check out this step-by-step tutorial on [building a Teams tab](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).</span></span>
- <span data-ttu-id="13937-173">Experimente os componentes no [playground.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="13937-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="13937-174">Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="13937-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="13937-175">Relatar bugs ou deixar uma solicitação de recurso [no GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="13937-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
