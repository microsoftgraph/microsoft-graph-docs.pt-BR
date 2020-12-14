---
title: Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph
description: Introdução à criação de um aplicativo Web usando o Microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664013"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="8b569-103">Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8b569-103">Build a web application with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8b569-104">Este tópico descreve como começar a usar o kit de ferramentas do Microsoft Graph em um aplicativo Web escrito no JavaScript da baunilha.</span><span class="sxs-lookup"><span data-stu-id="8b569-104">This topic describes how to get started with the Microsoft Graph Toolkit in a web application written in vanilla JavaScript.</span></span> <span data-ttu-id="8b569-105">Se quiser saber como usar o kit de ferramentas com uma estrutura da Web, consulte [compilar um aplicativo Web (reagir)](./use-toolkit-with-react.md) ou [compilar um aplicativo Web (angular)](./use-toolkit-with-angular.md).</span><span class="sxs-lookup"><span data-stu-id="8b569-105">If you would like to learn how to use the Toolkit with a web framework, see [Build a web app (React)](./use-toolkit-with-react.md) or [Build a web app (Angular)](./use-toolkit-with-angular.md).</span></span>

<span data-ttu-id="8b569-106">Introdução ao Microsoft Graph Toolkit envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="8b569-106">Getting started with the Microsoft Graph Toolkit involves the following steps:</span></span>
1. <span data-ttu-id="8b569-107">Adicione o Microsoft Graph Toolkit ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="8b569-107">Add Microsoft Graph Toolkit to your project.</span></span>
2. <span data-ttu-id="8b569-108">Inicialize o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="8b569-108">Initialize the MSAL Provider.</span></span>
3. <span data-ttu-id="8b569-109">Adicionar componentes.</span><span class="sxs-lookup"><span data-stu-id="8b569-109">Add components.</span></span>
4. <span data-ttu-id="8b569-110">Teste seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b569-110">Test your application.</span></span>

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a><span data-ttu-id="8b569-111">Adicionar o Microsoft Graph Toolkit ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="8b569-111">Add the Microsoft Graph Toolkit to your project</span></span>
<span data-ttu-id="8b569-112">Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.</span><span class="sxs-lookup"><span data-stu-id="8b569-112">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="8b569-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="8b569-113">unpkg</span></span>](#tab/html)
<span data-ttu-id="8b569-114">Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="8b569-114">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[<span data-ttu-id="8b569-115">npm</span><span class="sxs-lookup"><span data-stu-id="8b569-115">npm</span></span>](#tab/npm)
<span data-ttu-id="8b569-116">O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b569-116">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="8b569-117">Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="8b569-117">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```

---


> <span data-ttu-id="8b569-118">**Observação**: se você estiver direcionando um navegador como o IE11 que não ofereça suporte a componentes da Web nativamente, talvez seja necessário [incluir polipreenchimentos](./overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="8b569-118">**Note**: If you're targeting a browser such as IE11 that does not support web components natively, you might need to [include polyfills](./overview.md#polyfills).</span></span>

## <a name="initialize-the-msal-provider"></a><span data-ttu-id="8b569-119">Inicializar o provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="8b569-119">Initialize the MSAL Provider</span></span>
<span data-ttu-id="8b569-120">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="8b569-120">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="8b569-121">Para saber mais, consulte [usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="8b569-121">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="8b569-122">O [provedor MSAL](../providers/msal.md) usa MSAL.js para entrar em usuários e adquirir tokens.</span><span class="sxs-lookup"><span data-stu-id="8b569-122">The [MSAL Provider](../providers/msal.md) uses MSAL.js to sign in users and acquire tokens.</span></span> <span data-ttu-id="8b569-123">Você pode inicializar o provedor MSAL no HTML ou no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8b569-123">You can initialize the MSAL provider in your HTML or JavaScript.</span></span>

<span data-ttu-id="8b569-124">Se quiser usar sua própria autenticação de backend, use o provedor de [proxy](../providers/proxy.md) no lugar do provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="8b569-124">If you would like to use your own backend authentication, use the [Proxy Provider](../providers/proxy.md) in place of the MSAL provider.</span></span>

<span data-ttu-id="8b569-125">Você pode optar por inicializar o provedor em seu código HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8b569-125">You can choose to initialize the provider in either your HTML or your JavaScript code.</span></span> 

# <a name="html"></a>[<span data-ttu-id="8b569-126">formato</span><span class="sxs-lookup"><span data-stu-id="8b569-126">html</span></span>](#tab/HTML)
<span data-ttu-id="8b569-127">Adicione o `mgt-msal-provider` componente à sua página HTML e defina o `client-id` como seu cliente de aplicativo-ID.</span><span class="sxs-lookup"><span data-stu-id="8b569-127">Add the `mgt-msal-provider` component to your HTML page and set the `client-id` to your application client-id.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[<span data-ttu-id="8b569-128">JS</span><span class="sxs-lookup"><span data-stu-id="8b569-128">js</span></span>](#tab/JavaScript)
<span data-ttu-id="8b569-129">Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao aplicativo:</span><span class="sxs-lookup"><span data-stu-id="8b569-129">To initialize the MSAL provider in your JavaScript, add the following code to your application:</span></span>

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


<span data-ttu-id="8b569-130">A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais.</span><span class="sxs-lookup"><span data-stu-id="8b569-130">The client ID is the only property required to initialize the provider, but you can set additional options.</span></span> <span data-ttu-id="8b569-131">Para obter a lista completa, consulte [MSAL Provider](../providers/msal.md).</span><span class="sxs-lookup"><span data-stu-id="8b569-131">For the full list, see [Msal Provider](../providers/msal.md).</span></span>

### <a name="creating-an-appclient-id"></a><span data-ttu-id="8b569-132">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="8b569-132">Creating an app/client ID</span></span>
<span data-ttu-id="8b569-133">Para obter uma ID de cliente, você precisa [registrar seu aplicativo](./add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b569-133">In order to get a client ID, you need to [register your application](./add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="8b569-134">**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth.</span><span class="sxs-lookup"><span data-stu-id="8b569-134">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="8b569-135">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="8b569-135">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="8b569-136">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="8b569-136">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="add-components"></a><span data-ttu-id="8b569-137">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="8b569-137">Add components</span></span>
<span data-ttu-id="8b569-138">Depois de inicializar o provedor do MSAL, você pode começar a usar qualquer um dos componentes do kit de ferramentas.</span><span class="sxs-lookup"><span data-stu-id="8b569-138">After you initialize the MSAL provider, you can start using any of the Toolkit components.</span></span>

# <a name="html"></a>[<span data-ttu-id="8b569-139">formato</span><span class="sxs-lookup"><span data-stu-id="8b569-139">html</span></span>](#tab/HTML)
<span data-ttu-id="8b569-140">Veja a seguir um exemplo de trabalho completo usando o adMSAL-Loader, o provedor do inicializado em HTML e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="8b569-140">The following is a full working example using mgt-loader, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="8b569-141">Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado em HTML e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="8b569-141">This is an example using the ES6 modules, the MSAL Provider initialized in HTML, and the Login component:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[<span data-ttu-id="8b569-142">JS</span><span class="sxs-lookup"><span data-stu-id="8b569-142">js</span></span>](#tab/JavaScript)
<span data-ttu-id="8b569-143">Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado no JavaScript e o componente de logon:</span><span class="sxs-lookup"><span data-stu-id="8b569-143">This is an example using the ES6 modules, the MSAL Provider initialized in JavaScript, and the Login component:</span></span>

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


## <a name="test-your-app"></a><span data-ttu-id="8b569-144">Testar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b569-144">Test your app</span></span>

<span data-ttu-id="8b569-145">Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8b569-145">In order to test your app, MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> 

<span data-ttu-id="8b569-146">Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante.</span><span class="sxs-lookup"><span data-stu-id="8b569-146">If you're just getting started and want to play around, you can use [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code or any similar lightweight development server.</span></span> <span data-ttu-id="8b569-147">Baixe a extensão e abra o arquivo HTML usando o Live Server.</span><span class="sxs-lookup"><span data-stu-id="8b569-147">Download the extension and open your HTML file using live server.</span></span> 
> <span data-ttu-id="8b569-148">**Observação:** Certifique-se de que o **URI de redirecionamento** em seu registro de aplicativo está definido como a porta de localhost em que seu aplicativo está hospedado.</span><span class="sxs-lookup"><span data-stu-id="8b569-148">**Note:** Make sure the **redirect URI** in your app registration is set to the localhost port your application is hosted on.</span></span> <span data-ttu-id="8b569-149">Vá para o seu registro de aplicativo no [portal do Azure](https://portal.azure.com), clique em **autenticação** em gerenciar e adicione o **URI de redirecionamento** correto.</span><span class="sxs-lookup"><span data-stu-id="8b569-149">Go to your app registration in the [Azure portal](https://portal.azure.com), click **Authentication** under manage, and add the correct **redirect URI**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8b569-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8b569-150">Next Steps</span></span>
- <span data-ttu-id="8b569-151">Confira este tutorial passo a passo sobre como [criar um aplicativo Web simples](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span><span class="sxs-lookup"><span data-stu-id="8b569-151">Check out this step-by-step tutorial on [building a simple web app](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).</span></span>
- <span data-ttu-id="8b569-152">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="8b569-152">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="8b569-153">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="8b569-153">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="8b569-154">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="8b569-154">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>