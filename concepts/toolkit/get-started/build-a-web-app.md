---
title: Criar um aplicativo Web com o microsoft Graph Toolkit
description: Começar a criar um aplicativo Web usando o microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 5eed45974428a2c6daf47d02144741d937e12c91
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579897"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="f69e6-103">Criar um aplicativo Web com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f69e6-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f69e6-104">Este tópico descreve como começar a usar o microsoft Graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha.</span><span class="sxs-lookup"><span data-stu-id="f69e6-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="f69e6-105">Para obter um tutorial passo a passo, experimente o [módulo Introdução ao microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="f69e6-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="f69e6-106">Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a web app (React) ou](./use-toolkit-with-react.md) Build a Web app [(Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="f69e6-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="f69e6-107">Começar com o microsoft Graph Toolkit envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="f69e6-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="f69e6-108">Adicione o Microsoft Graph Toolkit ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="f69e6-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="f69e6-109">Inicializar o Provedor MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="f69e6-109">Initialize the MSAL 2.0 Provider.</span></span>
3. <span data-ttu-id="f69e6-110">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="f69e6-110">Add components.</span></span>
4. <span data-ttu-id="f69e6-111">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f69e6-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="f69e6-112">Adicionar o microsoft Graph Toolkit ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="f69e6-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="f69e6-113">Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="f69e6-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="f69e6-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="f69e6-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="f69e6-115">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="f69e6-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="f69e6-116">npm</span><span class="sxs-lookup"><span data-stu-id="f69e6-116">npm</span></span>](#tab/npm)
<span data-ttu-id="f69e6-117">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f69e6-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="f69e6-118">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="f69e6-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="f69e6-119">**Observação**: se você estiver direcionando um navegador como o IE11 que não dá suporte a componentes web na verdade, talvez seja necessário incluir [polífilos](./overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="f69e6-119">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-20-provider"></a><span data-ttu-id="f69e6-120">Inicializar o Provedor MSAL 2.0</span><span class="sxs-lookup"><span data-stu-id="f69e6-120">Initialize the MSAL 2.0 Provider</span></span>
<span data-ttu-id="f69e6-121">Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="f69e6-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="f69e6-122">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f69e6-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="f69e6-123">O [Provedor MSAL 2.0](../providers/msal2.md) usa o msal-browser para entrar nos usuários e adquirir tokens.</span><span class="sxs-lookup"><span data-stu-id="f69e6-123">The [MSAL 2.0 Provider](../providers/msal2.md) uses msal-browser to sign in users and acquire tokens.</span></span> <span data-ttu-id="f69e6-124">Você pode inicializar esse provedor em seu HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="f69e6-124">You can initialize this provider in your HTML or JavaScript.</span></span>

> <span data-ttu-id="f69e6-125">**Observação**: se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2.0, siga as etapas listadas [aqui](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span><span class="sxs-lookup"><span data-stu-id="f69e6-125">**Note**: If you are currently using MSAL Provider and would like to update to MSAL 2.0 Provider, follow the steps listed [here](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).</span></span>
<span data-ttu-id="f69e6-126">Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do provedor MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="f69e6-126">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL 2.0 provider.</span></span>

<span data-ttu-id="f69e6-127">Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript.</span><span class="sxs-lookup"><span data-stu-id="f69e6-127">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="f69e6-128">HTML</span><span class="sxs-lookup"><span data-stu-id="f69e6-128">html</span></span>](#tab/HTML)
<span data-ttu-id="f69e6-129">Adicione o `mgt-msal2-provider` componente à sua página HTML e desmarcar o para o seu aplicativo `client-id` client-id.</span><span class="sxs-lookup"><span data-stu-id="f69e6-129">Add the `mgt-msal2-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="js"></a>[<span data-ttu-id="f69e6-130">js</span><span class="sxs-lookup"><span data-stu-id="f69e6-130">js</span></span>](#tab/JavaScript)
<span data-ttu-id="f69e6-131">Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:</span><span class="sxs-lookup"><span data-stu-id="f69e6-131">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="f69e6-132">A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais.</span><span class="sxs-lookup"><span data-stu-id="f69e6-132">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="f69e6-133">Para ver a lista completa, consulte [Msal 2.0 Provider](../providers/msal2.md).</span><span class="sxs-lookup"><span data-stu-id="f69e6-133">For the full list, see [Msal 2.0 Provider](../providers/msal2.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="f69e6-134">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="f69e6-134">Creating an app/client ID</span></span>
<span data-ttu-id="f69e6-135">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f69e6-135">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="f69e6-136">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="f69e6-136">Add components</span></span>
<span data-ttu-id="f69e6-137">Depois de inicializar o provedor MSAL 2.0, você pode começar a usar qualquer um dos Toolkit componentes.</span><span class="sxs-lookup"><span data-stu-id="f69e6-137">After you initialize the MSAL 2.0 provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="f69e6-138">HTML</span><span class="sxs-lookup"><span data-stu-id="f69e6-138">html</span></span>](#tab/HTML)
<span data-ttu-id="f69e6-139">Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="f69e6-139">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="f69e6-140">Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="f69e6-140">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="f69e6-141">js</span><span class="sxs-lookup"><span data-stu-id="f69e6-141">js</span></span>](#tab/JavaScript)
<span data-ttu-id="f69e6-142">Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em JavaScript e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="f69e6-142">This is an example using the ES6 modules, the MSAL 2.0 Provider initialized in JavaScript, and the Login component:</span></span>

```js
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


## <a name="test-your-app"></a><span data-ttu-id="f69e6-143">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="f69e6-143">Test your app</span></span>

<span data-ttu-id="f69e6-144">Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f69e6-144">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="f69e6-145">Se você estiver apenas começando e quiser brincar, poderá usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante.</span><span class="sxs-lookup"><span data-stu-id="f69e6-145">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="f69e6-146">Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo.</span><span class="sxs-lookup"><span data-stu-id="f69e6-146">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="f69e6-147">**Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado.</span><span class="sxs-lookup"><span data-stu-id="f69e6-147">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="f69e6-148">Vá para o registro do aplicativo no [portal do Azure,](https://portal.azure.com)clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto.**</span><span class="sxs-lookup"><span data-stu-id="f69e6-148">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f69e6-149">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f69e6-149">Next Steps</span></span>
- <span data-ttu-id="f69e6-150">Confira o [tutorial Introdução ao Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.</span><span class="sxs-lookup"><span data-stu-id="f69e6-150">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="f69e6-151">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="f69e6-151">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="f69e6-152">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="f69e6-152">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="f69e6-153">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="f69e6-153">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
