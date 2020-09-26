---
title: Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph
description: Introdução à criação de um aplicativo Web usando o Microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 6852351e39aa3754ba7458bfe6fe5cd45f5cf635
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288523"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="74624-103">Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74624-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="74624-104">Este tópico descreve como começar a usar o kit de ferramentas do Microsoft Graph em um aplicativo Web escrito no JavaScript da baunilha.</span><span class="sxs-lookup"><span data-stu-id="74624-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="74624-105">Se quiser saber como usar o kit de ferramentas com uma estrutura da Web, confira [usar o kit de ferramentas com reagir](./use-toolkit-with-react.md) ou [usar o kit de ferramentas com angular](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="74624-105">If you would like to learn how to use the Toolkit with a web framework, see [Use the Toolkit with React](./use-toolkit-with-react.md) or [Use the Toolkit with Angular](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="74624-106">Introdução ao Microsoft Graph Toolkit envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="74624-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="74624-107">Adicione o Microsoft Graph Toolkit ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="74624-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="74624-108">Inicialize o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="74624-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="74624-109">Adicionar componentes.</span><span class="sxs-lookup"><span data-stu-id="74624-109">Add components.</span></span>
4. <span data-ttu-id="74624-110">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74624-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="74624-111">Adicionar o Microsoft Graph Toolkit ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="74624-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="74624-112">Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.</span><span class="sxs-lookup"><span data-stu-id="74624-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="74624-113">Usar via gerenciamento-carregador</span><span class="sxs-lookup"><span data-stu-id="74624-113">Use via mgt-loader</span></span>
<span data-ttu-id="74624-114">Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="74624-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="74624-115">Usar via NPM (módulos ES6)</span><span class="sxs-lookup"><span data-stu-id="74624-115">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="74624-116">O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74624-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="74624-117">Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="74624-117">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
> <span data-ttu-id="74624-118">**Observação**: se você estiver direcionando um navegador como o IE11 que não ofereça suporte a componentes da Web nativamente, talvez seja necessário [incluir polipreenchimentos](./overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="74624-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

<span data-ttu-id="74624-119">Agora, você pode fazer referência a todos os componentes do kit de ferramentas em seu aplicativo com:</span><span class="sxs-lookup"><span data-stu-id="74624-119">Now, you can reference the all the Toolkit components in your application with:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```
<span data-ttu-id="74624-120">Ou faça referência somente aos componentes que você precisa e Evite carregar tudo o mais.</span><span class="sxs-lookup"><span data-stu-id="74624-120">Or, reference only the components you need and avoid loading everything else.</span></span> <span data-ttu-id="74624-121">Por exemplo, para adicionar o provedor MSAL:</span><span class="sxs-lookup"><span data-stu-id="74624-121">For example, to add the MSAL Provider:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
```

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="74624-122">Inicializar o provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="74624-122">Initialize the MSAL Provider</span></span>
<span data-ttu-id="74624-123">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="74624-123">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="74624-124">Para saber mais, consulte [usando os provedores](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="74624-124">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="74624-125">O [provedor MSAL](../providers/msal.md) usa MSAL.js para entrar em usuários e adquirir tokens.</span><span class="sxs-lookup"><span data-stu-id="74624-125">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="74624-126">Você pode inicializar o provedor MSAL no HTML ou no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="74624-126">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="74624-127">Se quiser usar sua própria autenticação de backend, use o provedor de [proxy](../providers/proxy.md) no lugar do provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="74624-127">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="74624-128">Você pode optar por inicializar o provedor em seu código HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="74624-128">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="74624-129">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="74624-129">Initialize in your HTML page</span></span>
<span data-ttu-id="74624-130">Adicione o `mgt-msal-provider` componente à sua página HTML e defina o `client-id` como seu cliente de aplicativo-ID.</span><span class="sxs-lookup"><span data-stu-id="74624-130">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
### <a name="initialize-in-javascript"></a><span data-ttu-id="74624-131">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="74624-131">Initialize in JavaScript</span></span>
<span data-ttu-id="74624-132">Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao aplicativo:</span><span class="sxs-lookup"><span data-stu-id="74624-132">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```
<span data-ttu-id="74624-133">A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais.</span><span class="sxs-lookup"><span data-stu-id="74624-133">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="74624-134">Para obter a lista completa, consulte [MSAL Provider](../providers/msal.md).</span><span class="sxs-lookup"><span data-stu-id="74624-134">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="74624-135">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="74624-135">Creating an app/client ID</span></span>
<span data-ttu-id="74624-136">Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../../auth-register-app-v2.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="74624-136">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="74624-137">**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth.</span><span class="sxs-lookup"><span data-stu-id="74624-137">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="74624-138">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="74624-138">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="74624-139">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="74624-139">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="74624-140">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="74624-140">Add components</span></span>
<span data-ttu-id="74624-141">Depois de inicializar o provedor do MSAL, você pode começar a usar qualquer um dos componentes do kit de ferramentas.</span><span class="sxs-lookup"><span data-stu-id="74624-141">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

<span data-ttu-id="74624-142">Veja a seguir um exemplo de trabalho completo usando o adMSAL-Loader, o provedor do inicializado em HTML e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="74624-142">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="74624-143">Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado em HTML e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="74624-143">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="74624-144">Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado no JavaScript e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="74624-144">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

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

## <a name="test-your-app"></a><span data-ttu-id="74624-145">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="74624-145">Test your app</span></span>

<span data-ttu-id="74624-146">Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="74624-146">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="74624-147">Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante.</span><span class="sxs-lookup"><span data-stu-id="74624-147">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="74624-148">Baixe a extensão e abra o arquivo HTML usando o Live Server.</span><span class="sxs-lookup"><span data-stu-id="74624-148">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="74624-149">**Observação:** Certifique-se de que o **URI de redirecionamento** em seu registro de aplicativo está definido como a porta de localhost em que seu aplicativo está hospedado.</span><span class="sxs-lookup"><span data-stu-id="74624-149">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="74624-150">Vá para o seu registro de aplicativo no [portal do Azure](https://portal.azure.com), clique em **autenticação** em gerenciar e adicione o **URI de redirecionamento**correto.</span><span class="sxs-lookup"><span data-stu-id="74624-150">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="74624-151">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="74624-151">Next Steps</span></span>
- <span data-ttu-id="74624-152">Confira este tutorial passo a passo sobre como [criar um aplicativo Web simples](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span><span class="sxs-lookup"><span data-stu-id="74624-152">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="74624-153">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="74624-153">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="74624-154">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="74624-154">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="74624-155">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="74624-155">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>