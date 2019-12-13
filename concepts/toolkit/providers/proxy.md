---
title: Provedor de proxy
description: O provedor de proxy permite que você use sua própria autenticação do lado do servidor com o Microsoft Graph Toolkit.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 130811ded21013614c85cc90eea6f22c74e7cc73
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955768"
---
# <a name="proxy-provider"></a><span data-ttu-id="5ce5a-103">Provedor de proxy</span><span class="sxs-lookup"><span data-stu-id="5ce5a-103">Proxy provider</span></span>

<span data-ttu-id="5ce5a-104">Quando você usa o provedor de proxy, é possível usar a autenticação de backend (como o fluxo de autenticação em nome de 2.0) para alimentar o Microsoft Graph Toolkit encaminhando todas as chamadas para o Microsoft Graph através do seu próprio backend.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-104">When you use the proxy provider, you can use your backend authentication (such as Auth2.0 On-Behalf-Of flow) to power the Microsoft Graph Toolkit by routing all calls to Microsoft Graph through your own backend.</span></span>

<span data-ttu-id="5ce5a-105">Seu serviço de back-end deve expor uma API que será chamada para cada chamada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-105">Your backend service must expose an API that will be called for every call to Microsoft Graph.</span></span> <span data-ttu-id="5ce5a-106">Por exemplo, quando um componente tenta obter um recurso, o Proxyprovider chamará sua API base e acrescentará esse recurso.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-106">For example, when a component attempts to get a resource, the ProxyProvider will instead call your base API and append that resource.</span></span>

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

<span data-ttu-id="5ce5a-107">A implementação da API deve chamar o Microsoft Graph em nome do usuário e retornar os resultados para o componente.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-107">Your API implementation should then call Microsoft Graph on behalf of the user and return the results to the component.</span></span>

<span data-ttu-id="5ce5a-108">Para obter um exemplo de implementação, consulte o [exemplo MVC do ASP.net](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span><span class="sxs-lookup"><span data-stu-id="5ce5a-108">For an implementation example, see the [ASP.NET MVC sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc).</span></span> 

<span data-ttu-id="5ce5a-109">Para saber mais sobre provedores de autenticação, consulte [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="5ce5a-109">To learn more about authentication providers, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="5ce5a-110">Introdução</span><span class="sxs-lookup"><span data-stu-id="5ce5a-110">Get started</span></span>

<span data-ttu-id="5ce5a-111">Você pode inicializar o provedor de proxy no HTML ou no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-111">You can initialize the proxy provider in HTML or JavaScript.</span></span> <span data-ttu-id="5ce5a-112">Você deve fazer isso apenas uma vez por página.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-112">You should do this only once per page.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="5ce5a-113">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="5ce5a-113">Initialize in your HTML page</span></span>

<span data-ttu-id="5ce5a-114">Inicializar o provedor de proxy em HTML é a maneira mais simples de definir sua própria rota para autenticação personalizada no servidor.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-114">Initializing the proxy provider in HTML is the simplest way to define your own route for custom server-side authentication.</span></span> <span data-ttu-id="5ce5a-115">Use o `mgt-proxy-provider` componente para definir o **gráfico-proxy-URL**.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-115">Use the `mgt-proxy-provider` component to set the **graph-proxy-url**.</span></span> <span data-ttu-id="5ce5a-116">Isso definirá o provedor de proxy definido como o provedor global.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-116">This will set the defined proxy provider as the global provider.</span></span>

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| <span data-ttu-id="5ce5a-117">Atributo</span><span class="sxs-lookup"><span data-stu-id="5ce5a-117">Attribute</span></span> | <span data-ttu-id="5ce5a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ce5a-118">Description</span></span> |
| --- | --- |
| <span data-ttu-id="5ce5a-119">gráfico-proxy-URL</span><span class="sxs-lookup"><span data-stu-id="5ce5a-119">graph-proxy-url</span></span>  | <span data-ttu-id="5ce5a-120">URL base para a API de proxy.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-120">Base URL for the proxy API.</span></span> |


### <a name="initialize-in-javascript"></a><span data-ttu-id="5ce5a-121">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ce5a-121">Initialize in JavaScript</span></span>

<span data-ttu-id="5ce5a-122">Você pode fornecer mais opções inicializando o provedor no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-122">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

<span data-ttu-id="5ce5a-123">Opcionalmente, você pode enviar cabeçalhos adicionais com cada solicitação para a API de proxy usando uma função opcional como o segundo parâmetro no construtor.</span><span class="sxs-lookup"><span data-stu-id="5ce5a-123">Optionally, you can send additional headers with each request to your proxy api by using an optional function as the second parameter in the constructor.</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

<span data-ttu-id="5ce5a-124">Isso é útil quando você precisa passar tokens ou outros cabeçalhos para o back-end</span><span class="sxs-lookup"><span data-stu-id="5ce5a-124">This is useful when you need to pass tokens or other headers to your backend</span></span>

<span data-ttu-id="5ce5a-125">Se você estiver usando o `mgt-login` componente, também deverá especificar as `login` funções e `logout` para o provedor:</span><span class="sxs-lookup"><span data-stu-id="5ce5a-125">If you will be using the `mgt-login` component, you should also specify the `login` and `logout` functions for the provider:</span></span>

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

