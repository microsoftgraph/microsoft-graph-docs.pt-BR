---
title: Provedores de kit de ferramentas do Microsoft Graph
description: Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 221258b49d9a5217829633c7882b9dd4f9d2a221
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955782"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="bc8b8-103">Provedores de kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bc8b8-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="bc8b8-104">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="bc8b8-105">Cada provedor fornece uma implementação para adquirir o token de acesso necessário para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="bc8b8-106">Para que os componentes usem um provedor, você deve definir a `Providers.globalProvider` Propriedade como o valor de um provedor que você gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="bc8b8-107">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="bc8b8-108">O kit de ferramentas implementa os seguintes provedores:</span><span class="sxs-lookup"><span data-stu-id="bc8b8-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="bc8b8-109">MsalProvider</span><span class="sxs-lookup"><span data-stu-id="bc8b8-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="bc8b8-110">SharePointprovider</span><span class="sxs-lookup"><span data-stu-id="bc8b8-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="bc8b8-111">Teamprovider</span><span class="sxs-lookup"><span data-stu-id="bc8b8-111">TeamsProvider</span></span>](./providers/teams.md)
- [<span data-ttu-id="bc8b8-112">Proxyprovider</span><span class="sxs-lookup"><span data-stu-id="bc8b8-112">ProxyProvider</span></span>](./providers/proxy.md)
- [<span data-ttu-id="bc8b8-113">Simpleprovider</span><span class="sxs-lookup"><span data-stu-id="bc8b8-113">SimpleProvider</span></span>](./providers/custom.md)

<span data-ttu-id="bc8b8-114">Você pode criar um provedor a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-114">You can create a provider at any time.</span></span> <span data-ttu-id="bc8b8-115">Recomendamos que você crie o provedor antes de usar qualquer um dos componentes.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="bc8b8-116">Esta seção descreve como inicializar um provedor.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-116">This section describes how to initialize a provider.</span></span>

## <a name="providers-namespace"></a><span data-ttu-id="bc8b8-117">Namespace de provedores</span><span class="sxs-lookup"><span data-stu-id="bc8b8-117">Providers namespace</span></span>

<span data-ttu-id="bc8b8-118">O `Providers` namespace expõe as seguintes propriedades e funções:</span><span class="sxs-lookup"><span data-stu-id="bc8b8-118">The `Providers` namespace exposes the following properties and functions:</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="bc8b8-119">Defina essa propriedade como um provedor que você deseja usar globalmente.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-119">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="bc8b8-120">Todos os componentes usam essa propriedade para obter uma referência ao provedor.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-120">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="bc8b8-121">A definição dessa propriedade acionará `onProvidersChanged` o evento.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-121">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="bc8b8-122">A `callbackFunction` função será chamada quando um provedor for alterado ou quando o estado de um provedor for alterado.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-122">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="bc8b8-123">Um `ProvidersChangedState` valor de enumeração será passado para a função para indicar o que foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-123">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="bc8b8-124">Implementar seu próprio provedor</span><span class="sxs-lookup"><span data-stu-id="bc8b8-124">Implement your own provider</span></span>

<span data-ttu-id="bc8b8-125">O kit de ferramentas fornece duas maneiras de criar novos provedores:</span><span class="sxs-lookup"><span data-stu-id="bc8b8-125">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="bc8b8-126">Crie um novo `SimpleProvider` passando uma função para obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-126">Create a new `SimpleProvider` by passing in a function for getting an access token.</span></span>
- <span data-ttu-id="bc8b8-127">Estenda a `IProvider` classe abstract.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-127">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="bc8b8-128">Para obter mais detalhes sobre cada um, consulte [Custom Providers](./providers/custom.md).</span><span class="sxs-lookup"><span data-stu-id="bc8b8-128">For more details about each one, see [custom providers](./providers/custom.md).</span></span>

## <a name="using-multiple-providers"></a><span data-ttu-id="bc8b8-129">Usando vários provedores</span><span class="sxs-lookup"><span data-stu-id="bc8b8-129">Using multiple providers</span></span>

<span data-ttu-id="bc8b8-130">Em alguns cenários, seu aplicativo será executado em um ambiente diferente e exigirá um provedor diferente.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-130">In some scenarios, your application will run in a different environment and require a different provider.</span></span> <span data-ttu-id="bc8b8-131">Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, e você pode precisar usar o MsalProvider e o Teamprovider.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-131">For example, the app might run as both a web application and a Microsoft Teams tab and you might need to use the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="bc8b8-132">Para este cenário, todos os componentes do provedor `depends-on` têm o atributo para criar uma cadeia de fallback, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-132">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="bc8b8-133">Neste cenário, o MsalProvider será usado somente se o Teams não estiver disponível no ambiente atual.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-133">In this scenario, the MsalProvider will only be used if the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="bc8b8-134">Para fazer o mesmo no código, você pode usar a `isAvailable` Propriedade no provedor, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-134">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="bc8b8-135">Fazendo suas próprias chamadas para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bc8b8-135">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="bc8b8-136">Todos os componentes podem acessar o Microsoft Graph sem a necessidade de personalização, desde que você inicialize um provedor (conforme descrito na seção anterior).</span><span class="sxs-lookup"><span data-stu-id="bc8b8-136">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="bc8b8-137">Para obter uma referência para o mesmo SDK do Microsoft Graph usado pelos componentes, primeiro obtenha uma referência para o IProvider global e, em seguida `Graph` , use o objeto, conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="bc8b8-137">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="bc8b8-138">Pode haver casos em que você precisará transmitir permissões adicionais, dependendo da API que você está chamando.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-138">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="bc8b8-139">O `graph` objeto é uma instância do [SDK do JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) e você pode usá-lo para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-139">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
