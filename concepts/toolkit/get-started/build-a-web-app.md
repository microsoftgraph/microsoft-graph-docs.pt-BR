---
title: Criar um aplicativo Web com o Microsoft Graph Toolkit
description: Começar a criar um aplicativo Web usando o microsoft graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 974f6351bdce985089d93f607210c8eb47b902ba
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961349"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="5db2b-103">Criar um aplicativo Web com o Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="5db2b-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5db2b-104">Este tópico descreve como começar a usar o microsoft graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha.</span><span class="sxs-lookup"><span data-stu-id="5db2b-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="5db2b-105">Para obter um tutorial passo a passo, experimente o [módulo Introdução ao Microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="5db2b-105">For a step-by-step tutorial, try the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> <span data-ttu-id="5db2b-106">Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a Web app (React)](./use-toolkit-with-react.md) ou Build a Web app [(Angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="5db2b-106">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="5db2b-107">Começar a trabalhar com o Microsoft Graph Toolkit as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="5db2b-107">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="5db2b-108">Adicione o Microsoft Graph Toolkit ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="5db2b-108">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="5db2b-109">Inicializar o Provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="5db2b-109">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="5db2b-110">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="5db2b-110">Add components.</span></span>
4. <span data-ttu-id="5db2b-111">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5db2b-111">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="5db2b-112">Adicionar o microsoft graph Toolkit ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="5db2b-112">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="5db2b-113">Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="5db2b-113">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="5db2b-114">unpkg</span><span class="sxs-lookup"><span data-stu-id="5db2b-114">unpkg</span></span>](#tab/html)
<span data-ttu-id="5db2b-115">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="5db2b-115">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="5db2b-116">npm</span><span class="sxs-lookup"><span data-stu-id="5db2b-116">npm</span></span>](#tab/npm)
<span data-ttu-id="5db2b-117">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5db2b-117">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="5db2b-118">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="5db2b-118">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="5db2b-119">**Observação**: se você estiver direcionando um navegador como o IE11 que não dá suporte a componentes web na verdade, talvez seja necessário incluir [polífilos](./overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="5db2b-119">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="5db2b-120">Inicializar o provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="5db2b-120">Initialize the MSAL Provider</span></span>
<span data-ttu-id="5db2b-121">Os provedores Toolkit Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="5db2b-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="5db2b-122">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="5db2b-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="5db2b-123">O [Provedor MSAL](../providers/msal.md) usa MSAL.js para entrar em usuários e adquirir tokens.</span><span class="sxs-lookup"><span data-stu-id="5db2b-123">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="5db2b-124">Você pode inicializar o provedor MSAL em seu HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5db2b-124">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="5db2b-125">Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="5db2b-125">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="5db2b-126">Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5db2b-126">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="5db2b-127">HTML</span><span class="sxs-lookup"><span data-stu-id="5db2b-127">html</span></span>](#tab/HTML)
<span data-ttu-id="5db2b-128">Adicione o `mgt-msal-provider` componente à sua página HTML e desmarcar o para o seu aplicativo `client-id` client-id.</span><span class="sxs-lookup"><span data-stu-id="5db2b-128">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[<span data-ttu-id="5db2b-129">js</span><span class="sxs-lookup"><span data-stu-id="5db2b-129">js</span></span>](#tab/JavaScript)
<span data-ttu-id="5db2b-130">Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:</span><span class="sxs-lookup"><span data-stu-id="5db2b-130">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="5db2b-131">A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais.</span><span class="sxs-lookup"><span data-stu-id="5db2b-131">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="5db2b-132">Para ver a lista completa, consulte [Msal Provider](../providers/msal.md).</span><span class="sxs-lookup"><span data-stu-id="5db2b-132">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="5db2b-133">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="5db2b-133">Creating an app/client ID</span></span>
<span data-ttu-id="5db2b-134">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5db2b-134">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="5db2b-135">**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="5db2b-135">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="5db2b-136">Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="5db2b-136">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="5db2b-137">Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="5db2b-137">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="5db2b-138">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="5db2b-138">Add components</span></span>
<span data-ttu-id="5db2b-139">Depois de inicializar o provedor MSAL, você pode começar a usar qualquer um dos componentes Toolkit de dados.</span><span class="sxs-lookup"><span data-stu-id="5db2b-139">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="5db2b-140">HTML</span><span class="sxs-lookup"><span data-stu-id="5db2b-140">html</span></span>](#tab/HTML)
<span data-ttu-id="5db2b-141">Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="5db2b-141">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="5db2b-142">Este é um exemplo usando os módulos ES6, o Provedor MSAL inicializado em HTML e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="5db2b-142">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="5db2b-143">js</span><span class="sxs-lookup"><span data-stu-id="5db2b-143">js</span></span>](#tab/JavaScript)
<span data-ttu-id="5db2b-144">Este é um exemplo usando os módulos ES6, o Provedor MSAL inicializado em JavaScript e o componente logon:</span><span class="sxs-lookup"><span data-stu-id="5db2b-144">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
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


## <a name="test-your-app"></a><span data-ttu-id="5db2b-145">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="5db2b-145">Test your app</span></span>

<span data-ttu-id="5db2b-146">Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="5db2b-146">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="5db2b-147">Se você estiver apenas começando e quiser brincar, pode usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no código Visual Studio ou em qualquer servidor de desenvolvimento leve semelhante.</span><span class="sxs-lookup"><span data-stu-id="5db2b-147">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="5db2b-148">Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo.</span><span class="sxs-lookup"><span data-stu-id="5db2b-148">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="5db2b-149">**Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado.</span><span class="sxs-lookup"><span data-stu-id="5db2b-149">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="5db2b-150">Vá para o registro do aplicativo no [portal do Azure,](https://portal.azure.com)clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto.**</span><span class="sxs-lookup"><span data-stu-id="5db2b-150">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5db2b-151">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="5db2b-151">Next Steps</span></span>
- <span data-ttu-id="5db2b-152">Confira o [tutorial Introdução ao Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.</span><span class="sxs-lookup"><span data-stu-id="5db2b-152">Check out the [Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) step-by-step tutorial.</span></span>
- <span data-ttu-id="5db2b-153">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="5db2b-153">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="5db2b-154">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="5db2b-154">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="5db2b-155">Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="5db2b-155">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
