---
title: Provedores de kit de ferramentas do Microsoft Graph
description: Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 52b0510fdc79253cb2a448b7a454b1dcfaf01bb9
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275721"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="344e1-103">Provedores de kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="344e1-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="344e1-104">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="344e1-104">The Microsoft Graph Toolkit providers enable authentication and Microsoft Graph access for all components.</span></span> <span data-ttu-id="344e1-105">Cada provedor fornece uma implementação para adquirir o token de acesso necessário para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="344e1-105">Each provider provides implementation for acquiring the necessary access token for calling the Microsoft Graph APIs.</span></span>

<span data-ttu-id="344e1-106">Para que os componentes usem um provedor, você deve definir a `Providers.globalProvider` Propriedade como o valor de um provedor que você gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="344e1-106">For the components to use a provider, you must set the `Providers.globalProvider` property to the value for a provider you'd like to use.</span></span>

<span data-ttu-id="344e1-107">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="344e1-107">The following example shows how to use the MsalProvider.</span></span>

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

<span data-ttu-id="344e1-108">O kit de ferramentas implementa os seguintes provedores:</span><span class="sxs-lookup"><span data-stu-id="344e1-108">The toolkit implements the following providers:</span></span>

- [<span data-ttu-id="344e1-109">MsalProvider</span><span class="sxs-lookup"><span data-stu-id="344e1-109">MsalProvider</span></span>](./providers/msal.md)
- [<span data-ttu-id="344e1-110">SharePointprovider</span><span class="sxs-lookup"><span data-stu-id="344e1-110">SharePointProvider</span></span>](./providers/sharepoint.md)
- [<span data-ttu-id="344e1-111">Teamprovider</span><span class="sxs-lookup"><span data-stu-id="344e1-111">TeamsProvider</span></span>](./providers/teams.md)
- <span data-ttu-id="344e1-112">Provedor de suplementos do Office (em breve)</span><span class="sxs-lookup"><span data-stu-id="344e1-112">Office Add-ins provider (coming soon)</span></span>

## <a name="get-started"></a><span data-ttu-id="344e1-113">Introdução</span><span class="sxs-lookup"><span data-stu-id="344e1-113">Get started</span></span>

<span data-ttu-id="344e1-114">Você pode criar um provedor a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="344e1-114">You can create a provider at any time.</span></span> <span data-ttu-id="344e1-115">Recomendamos que você crie o provedor antes de usar qualquer um dos componentes.</span><span class="sxs-lookup"><span data-stu-id="344e1-115">We recommend that you create the provider before you use any of the components.</span></span> <span data-ttu-id="344e1-116">Esta seção descreve como inicializar um provedor.</span><span class="sxs-lookup"><span data-stu-id="344e1-116">This section describes how to initialize a provider.</span></span>

<span data-ttu-id="344e1-117">A `Providers` variável global expõe as seguintes propriedades e funções</span><span class="sxs-lookup"><span data-stu-id="344e1-117">The `Providers` global variable exposes the following properties and functions</span></span>

- `globalProvider : IProvider`

<span data-ttu-id="344e1-118">Defina essa propriedade como um provedor que você deseja usar globalmente.</span><span class="sxs-lookup"><span data-stu-id="344e1-118">Set this property to a provider that you want to use globally.</span></span> <span data-ttu-id="344e1-119">Todos os componentes usam essa propriedade para obter uma referência ao provedor.</span><span class="sxs-lookup"><span data-stu-id="344e1-119">All components use this property to get a reference to the provider.</span></span> <span data-ttu-id="344e1-120">A definição dessa propriedade acionará `onProvidersChanged` o evento.</span><span class="sxs-lookup"><span data-stu-id="344e1-120">Setting this property will fire the `onProvidersChanged` event.</span></span>

- `function onProviderUpdated(callbackFunction)`

<span data-ttu-id="344e1-121">A `callbackFunction` função será chamada quando um provedor for alterado ou quando o estado de um provedor for alterado.</span><span class="sxs-lookup"><span data-stu-id="344e1-121">The `callbackFunction` function will be called when a provider is changed or when the state of a provider changes.</span></span> <span data-ttu-id="344e1-122">Um `ProvidersChangedState` valor de enumeração será passado para a função para indicar o que foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="344e1-122">A `ProvidersChangedState` enum value will be passed to the function to indicate what updated.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="344e1-123">Implementar seu próprio provedor</span><span class="sxs-lookup"><span data-stu-id="344e1-123">Implement your own provider</span></span>

<span data-ttu-id="344e1-124">O kit de ferramentas fornece duas maneiras de criar novos provedores:</span><span class="sxs-lookup"><span data-stu-id="344e1-124">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="344e1-125">Criar um novo `SimpleProvider` passando uma função para obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="344e1-125">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="344e1-126">Estender a `IProvider` classe abstrata</span><span class="sxs-lookup"><span data-stu-id="344e1-126">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="344e1-127">Leia mais sobre cada um na documentação dos [provedores personalizados](./providers/custom.md) .</span><span class="sxs-lookup"><span data-stu-id="344e1-127">Read more about each one in the [custom providers](./providers/custom.md) documentation.</span></span>

## <a name="using-multiple-providers"></a><span data-ttu-id="344e1-128">Usando vários provedores</span><span class="sxs-lookup"><span data-stu-id="344e1-128">Using multiple providers</span></span>

<span data-ttu-id="344e1-129">Em alguns cenários, seu aplicativo será executado em um ambiente diferente e exigirá um provedor diferente.</span><span class="sxs-lookup"><span data-stu-id="344e1-129">In some scenarios your application will run in a different environment and require a different provider.</span></span> <span data-ttu-id="344e1-130">Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, e você pode precisar usar o MsalProvider e o Teamprovider.</span><span class="sxs-lookup"><span data-stu-id="344e1-130">For example, the app might run as both a web application and a Microsoft Teams tab and you might need to use the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="344e1-131">Para este cenário, todos os componentes do provedor `depends-on` têm o atributo para criar uma cadeia de fallback, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="344e1-131">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="344e1-132">Neste cenário, o MsalProvider será usado somente se o Teams não estiver disponível no ambiente atual.</span><span class="sxs-lookup"><span data-stu-id="344e1-132">In this scenario, the MsalProvider will only be used if the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="344e1-133">Para fazer o mesmo no código, você pode usar a `isAvailable` Propriedade no provedor, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="344e1-133">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="344e1-134">Fazendo suas próprias chamadas para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="344e1-134">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="344e1-135">Todos os componentes podem acessar o Microsoft Graph sem a necessidade de personalização, desde que você inicialize um provedor (conforme descrito na seção anterior).</span><span class="sxs-lookup"><span data-stu-id="344e1-135">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous section).</span></span> <span data-ttu-id="344e1-136">Para obter uma referência para o mesmo SDK do Microsoft Graph usado pelos componentes, primeiro obtenha uma referência para o IProvider global e, em seguida `Graph` , use o objeto, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="344e1-136">To get a reference to the same Microsoft Graph SDK used by the components, first get a reference to the global IProvider and then use the `Graph` object, as shown.</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

<span data-ttu-id="344e1-137">Pode haver casos em que você precisará transmitir permissões adicionais, dependendo da API que você está chamando.</span><span class="sxs-lookup"><span data-stu-id="344e1-137">There might be cases were you will need to pass additional permissions, depending on the API you're calling.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

<span data-ttu-id="344e1-138">O `graph` objeto é uma instância do [SDK do JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) e você pode usá-lo para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="344e1-138">The `graph` object is an instance of the [Microsoft Graph Javascript SDK](https://github.com/microsoftgraph/msgraph-sdk-javascript) and you can use it to make any calls to Microsoft Graph.</span></span>
