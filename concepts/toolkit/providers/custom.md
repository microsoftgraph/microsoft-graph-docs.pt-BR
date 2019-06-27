---
title: Provedor personalizado
description: Crie um provedor personalizado para habilitar a autenticação e o acesso de gráfico para os componentes do Microsoft Graph Toolkit, se você tiver um código de autenticação existente em seu aplicativo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: acd96e6dc7e13b1e1fbfc5353e3db2132a23e246
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242941"
---
# <a name="custom-provider"></a><span data-ttu-id="ff59e-103">Provedor personalizado</span><span class="sxs-lookup"><span data-stu-id="ff59e-103">Custom provider</span></span>

<span data-ttu-id="ff59e-104">Se você tiver um código de autenticação existente em seu aplicativo, poderá criar um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph para os componentes do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="ff59e-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="ff59e-105">Há duas maneiras de criar provedores personalizados:</span><span class="sxs-lookup"><span data-stu-id="ff59e-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="ff59e-106">Criar um novo `SimpleProvider` passando uma função para obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="ff59e-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="ff59e-107">Estender a `IProvider` classe abstrata</span><span class="sxs-lookup"><span data-stu-id="ff59e-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="ff59e-108">Este artigo descreve cada abordagem em mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="ff59e-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="ff59e-109">Simpleprovider</span><span class="sxs-lookup"><span data-stu-id="ff59e-109">SimpleProvider</span></span>

<span data-ttu-id="ff59e-110">Crie uma `SimpleProvider` instância da classe passando uma função que retornará um token de acesso para escopos aprovados.</span><span class="sxs-lookup"><span data-stu-id="ff59e-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span>

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="ff59e-111">Além disso, você também pode fornecer uma função `login` opcional `logout` e que possa lidar com as chamadas de entrada e de saída do componente de [logon](../components/login.md) .</span><span class="sxs-lookup"><span data-stu-id="ff59e-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  // login code
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a><span data-ttu-id="ff59e-112">Gerenciar estado</span><span class="sxs-lookup"><span data-stu-id="ff59e-112">Manage state</span></span>

<span data-ttu-id="ff59e-113">Para que os componentes estejam cientes do estado do provedor, será necessário chamar o `provider.setState(state: ProviderState)` método sempre que o estado for alterado.</span><span class="sxs-lookup"><span data-stu-id="ff59e-113">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="ff59e-114">Por exemplo, quando o usuário entrou, ligue `provider.setState(ProviderState.SignedIn)`para.</span><span class="sxs-lookup"><span data-stu-id="ff59e-114">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="ff59e-115">A `ProviderState` enumeração define três Estados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="ff59e-115">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="ff59e-116">IProvider</span><span class="sxs-lookup"><span data-stu-id="ff59e-116">IProvider</span></span>

<span data-ttu-id="ff59e-117">Você pode estender a `IProvider` classe abstract para criar seu próprio provedor.</span><span class="sxs-lookup"><span data-stu-id="ff59e-117">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="ff59e-118">Estado</span><span class="sxs-lookup"><span data-stu-id="ff59e-118">State</span></span>

<span data-ttu-id="ff59e-119">Um provedor deve acompanhar o estado de autenticação e atualizar os componentes quando o estado for alterado.</span><span class="sxs-lookup"><span data-stu-id="ff59e-119">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="ff59e-120">A `IProvider` classe já implementa o `onStateChanged(eventHandler)` manipulador e a `state: ProviderState` propriedade.</span><span class="sxs-lookup"><span data-stu-id="ff59e-120">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="ff59e-121">Você só precisa usar o `setState(state:ProviderState)` método na sua implementação para atualizar o estado quando ele for alterado.</span><span class="sxs-lookup"><span data-stu-id="ff59e-121">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="ff59e-122">A atualização do estado acionará `stateChanged` o evento e atualizará todos os componentes automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ff59e-122">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="ff59e-123">Login/logout</span><span class="sxs-lookup"><span data-stu-id="ff59e-123">Login/Logout</span></span>

<span data-ttu-id="ff59e-124">Se seu provedor fornece a funcionalidade de logon ou logout, `login(): Promise<void>` implemente os métodos e `logout(): Promise<void>` .</span><span class="sxs-lookup"><span data-stu-id="ff59e-124">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="ff59e-125">Esses métodos são opcionais.</span><span class="sxs-lookup"><span data-stu-id="ff59e-125">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="ff59e-126">Token de acesso</span><span class="sxs-lookup"><span data-stu-id="ff59e-126">Access token</span></span>

<span data-ttu-id="ff59e-127">Você deve implementar o `getAccessToken({'scopes': scopes[]}) : Promise<string>` método.</span><span class="sxs-lookup"><span data-stu-id="ff59e-127">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="ff59e-128">Este método é usado para obter um token válido antes de cada chamada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff59e-128">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="ff59e-129">Graficamente</span><span class="sxs-lookup"><span data-stu-id="ff59e-129">Graph</span></span>

<span data-ttu-id="ff59e-130">Os componentes usam o SDK do JavaScript do Microsoft Graph para todas as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff59e-130">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="ff59e-131">Seu provedor deve tornar o SDK disponível por meio `graph` da propriedade.</span><span class="sxs-lookup"><span data-stu-id="ff59e-131">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="ff59e-132">No construtor, crie uma nova `Graph` instância, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="ff59e-132">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="ff59e-133">A `Graph` classe é um invólucro claro na parte superior do SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff59e-133">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="ff59e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff59e-134">Example</span></span>

<span data-ttu-id="ff59e-135">Todos os provedores estendem a `IProvider` classe abstrata.</span><span class="sxs-lookup"><span data-stu-id="ff59e-135">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="ff59e-136">Para obter exemplos, dê uma olhada no código-fonte de qualquer um dos [provedores existentes](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span><span class="sxs-lookup"><span data-stu-id="ff59e-136">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="ff59e-137">Definir o provedor global</span><span class="sxs-lookup"><span data-stu-id="ff59e-137">Set the global provider</span></span>

<span data-ttu-id="ff59e-138">Os componentes usam `Providers.globalProvider` a propriedade para acessar um provedor.</span><span class="sxs-lookup"><span data-stu-id="ff59e-138">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="ff59e-139">Depois de criar seu próprio provedor, defina essa propriedade como seu provedor.</span><span class="sxs-lookup"><span data-stu-id="ff59e-139">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="ff59e-140">Todos os componentes serão notificados do novo provedor e começarão a usá-lo.</span><span class="sxs-lookup"><span data-stu-id="ff59e-140">All the components will be notified of the new provider and start using it.</span></span>
