---
title: Criar um aplicativo Web com o microsoft Graph Toolkit
description: Começar a criar um aplicativo Web usando o microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 989e79c2b52f7e02fb61604d3011f13aced580ed
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941533"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="3c502-103">Criar um aplicativo Web com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3c502-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3c502-104">Este tópico descreve como começar a usar o microsoft Graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha.</span><span class="sxs-lookup"><span data-stu-id="3c502-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="3c502-105">Para obter um tutorial passo a passo, experimente o [módulo Introdução ao microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="3c502-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="3c502-106">Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a web app (React) ou](./use-toolkit-with-react.md) Build a Web app [(Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="3c502-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="3c502-107">Começar com o microsoft Graph Toolkit envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="3c502-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="3c502-108">Adicione o Microsoft Graph Toolkit ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="3c502-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="3c502-109">Inicializar o Provedor MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="3c502-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="3c502-110">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="3c502-110">Add components.</span></span>
4. <span data-ttu-id="3c502-111">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c502-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="3c502-112">Adicionar o microsoft Graph Toolkit ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="3c502-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="3c502-113">Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="3c502-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="3c502-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="3c502-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="3c502-115">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="3c502-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="3c502-116">npm</span><span class="sxs-lookup"><span data-stu-id="3c502-116">npm</span></span>](#tab/npm)
<span data-ttu-id="3c502-117">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3c502-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="3c502-118">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="3c502-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="3c502-119">Inicializar o Provedor MSAL 2.0</span><span class="sxs-lookup"><span data-stu-id="3c502-119">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="3c502-120">Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="3c502-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="3c502-121">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="3c502-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="3c502-122">O [Provedor MSAL 2.0](../providers/msal2.md) usa o msal-browser para entrar nos usuários e adquirir tokens.</span><span class="sxs-lookup"><span data-stu-id="3c502-122">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="3c502-123">Você pode inicializar esse provedor em seu HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3c502-123">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="3c502-124">**Observação**: se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2.0, siga as etapas listadas [aqui](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span><span class="sxs-lookup"><span data-stu-id="3c502-124">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="3c502-125">Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do provedor MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="3c502-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="3c502-126">Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3c502-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="3c502-127">HTML</span><span class="sxs-lookup"><span data-stu-id="3c502-127">HTML</span></span>](#tab/HTML)
<span data-ttu-id="3c502-128">Adicione o `mgt-msal2-provider` componente à sua página HTML e desmarcar o para o seu aplicativo `client-id` client-id.</span><span class="sxs-lookup"><span data-stu-id="3c502-128">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="javascript"></a>[<span data-ttu-id="3c502-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c502-129">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="3c502-130">Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:</span><span class="sxs-lookup"><span data-stu-id="3c502-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```javascript
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="3c502-131">A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais.</span><span class="sxs-lookup"><span data-stu-id="3c502-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="3c502-132">Para ver a lista completa, consulte [Msal 2.0 Provider](../providers/msal2.md).</span><span class="sxs-lookup"><span data-stu-id="3c502-132">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="3c502-133">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="3c502-133">Creating an app/client ID</span></span>
<span data-ttu-id="3c502-134">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c502-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="3c502-135">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="3c502-135">Add components</span></span>
<span data-ttu-id="3c502-136">Depois de inicializar o provedor MSAL 2.0, você pode começar a usar qualquer um dos Toolkit componentes.</span><span class="sxs-lookup"><span data-stu-id="3c502-136">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="3c502-137">HTML</span><span class="sxs-lookup"><span data-stu-id="3c502-137">HTML</span></span>](#tab/HTML)
<span data-ttu-id="3c502-138">Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="3c502-138">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="3c502-139">Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="3c502-139">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="javascript"></a>[<span data-ttu-id="3c502-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c502-140">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="3c502-141">Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em JavaScript e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="3c502-141">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```javascript
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a><span data-ttu-id="3c502-142">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c502-142">Test your app</span></span>

<span data-ttu-id="3c502-143">Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3c502-143">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="3c502-144">Se você estiver apenas começando e quiser brincar, poderá usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante.</span><span class="sxs-lookup"><span data-stu-id="3c502-144">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="3c502-145">Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo.</span><span class="sxs-lookup"><span data-stu-id="3c502-145">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="3c502-146">**Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado.</span><span class="sxs-lookup"><span data-stu-id="3c502-146">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="3c502-147">Vá para o registro do aplicativo no [portal do Azure,](https://portal.azure.com)clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto.**</span><span class="sxs-lookup"><span data-stu-id="3c502-147">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="track-a-users-sign-in-state"></a><span data-ttu-id="3c502-148">Rastrear o estado de login de um usuário</span><span class="sxs-lookup"><span data-stu-id="3c502-148">Track a user's sign in state</span></span>

<span data-ttu-id="3c502-149">Você pode detectar quando um usuário se inscreveu com êxito e exibiu componentes específicos de acordo.</span><span class="sxs-lookup"><span data-stu-id="3c502-149">You can detect when a user has successfully signed in and display specific components accordingly.</span></span> <span data-ttu-id="3c502-150">Por exemplo, exibe o componente de agenda se o usuário tiver se assinado.</span><span class="sxs-lookup"><span data-stu-id="3c502-150">For example, display the agenda component if the user has signed in.</span></span> <span data-ttu-id="3c502-151">Caso contrário, exibe a interface de login.</span><span class="sxs-lookup"><span data-stu-id="3c502-151">Otherwise, display the sign in interface.</span></span>

<span data-ttu-id="3c502-152">Você pode determinar se um usuário está assinado avaliando `globalProvider` e `providerState` .</span><span class="sxs-lookup"><span data-stu-id="3c502-152">You can determine if a user is signed in by evaluating the `globalProvider` and `providerState`.</span></span>

# <a name="html"></a>[<span data-ttu-id="3c502-153">HTML</span><span class="sxs-lookup"><span data-stu-id="3c502-153">HTML</span></span>](#tab/HTML)

<span data-ttu-id="3c502-154">Se você estiver usando a `mgt-loader` biblioteca, poderá acessar e `provider` a partir `providerState` da `mgt` propriedade.</span><span class="sxs-lookup"><span data-stu-id="3c502-154">If you're using the `mgt-loader` library, you can access the `provider` and `providerState` from the `mgt` property.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<div id="main"><mgt-login></mgt-login></div>

<script>
    const provider = mgt.Providers.globalProvider;
    const isLoggedIn = provider && provider.state === mgt.ProviderState.SignedIn

    // Show the mgt-agenda component ONLY if the user is logged in, show the mgt-login component if not
    function loadAgenda(){
        if(isLoggedIn){
            const main = document.getElementById("main");
            main.innerHTML = `<mgt-agenda></mgt-agenda>`;
        } else {
            main.innerHTML = `<mgt-login></mgt-login>`;
        }
    }

    loadAgenda();
</script>
```

# <a name="javascript"></a>[<span data-ttu-id="3c502-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c502-155">JavaScript</span></span>](#tab/JavaScript)
<span data-ttu-id="3c502-156">Se você estiver usando o Toolkit por meio dos pacotes npm, poderá importar `provider` o e `providerState` de `@microsoft/mgt` .</span><span class="sxs-lookup"><span data-stu-id="3c502-156">If you're using the Toolkit via the npm packages, you can import the `provider` and `providerState` from `@microsoft/mgt`.</span></span>

```javascript
import {Providers, ProviderState} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})

function isLoggedIn(){
    const provider = Providers.globalProvider;
    return provider && provider.state === ProviderState.SignedIn;
}

function loadAgenda(){
    const agenda = document.createElement("mgt-agenda");
    const loginComponent = document.createElement("mgt-login");
    if(isLoggedIn()){
        // the user is logged in, load their agenda
        document.body.innerHTML = `<mgt-agenda></mgt-agenda>`;
    } else {
        // the user is not logged in, show them the login component
        document.body.innerHTML = `<mgt-login></mgt-login>`
    }
}

loadAgenda();
```

---


## <a name="next-steps"></a><span data-ttu-id="3c502-157">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3c502-157">Next Steps</span></span>
- <span data-ttu-id="3c502-158">Confira o [tutorial Introdução ao Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.</span><span class="sxs-lookup"><span data-stu-id="3c502-158">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="3c502-159">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="3c502-159">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="3c502-160">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="3c502-160">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="3c502-161">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="3c502-161">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
