---
title: Provedor personalizado
description: Crie um provedor personalizado para habilitar a autenticação e o acesso de gráfico para os componentes do Microsoft Graph Toolkit, se você tiver um código de autenticação existente em seu aplicativo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 57b7ca843f71d22992df18dc2466d0182d3fc556
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086596"
---
# <a name="custom-provider"></a><span data-ttu-id="47075-103">Provedor personalizado</span><span class="sxs-lookup"><span data-stu-id="47075-103">Custom provider</span></span>

<span data-ttu-id="47075-104">Se você tiver um código de autenticação existente em seu aplicativo, poderá criar um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph para os componentes do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="47075-104">If you have existing authentication code in your application, you can create a custom provider to enable authentication and access to Microsoft Graph for Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="47075-105">Há duas maneiras de criar provedores personalizados:</span><span class="sxs-lookup"><span data-stu-id="47075-105">There are two ways to create custom providers:</span></span>

- <span data-ttu-id="47075-106">Criar um novo `SimpleProvider` passando uma função para obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="47075-106">Create a new `SimpleProvider` by passing in a function for getting an access token</span></span>
- <span data-ttu-id="47075-107">Estender a `IProvider` classe abstrata</span><span class="sxs-lookup"><span data-stu-id="47075-107">Extend the `IProvider` abstract class</span></span>

<span data-ttu-id="47075-108">Este artigo descreve cada abordagem em mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="47075-108">This article describes each approach in more detail.</span></span>

## <a name="simpleprovider"></a><span data-ttu-id="47075-109">Simpleprovider</span><span class="sxs-lookup"><span data-stu-id="47075-109">SimpleProvider</span></span>

<span data-ttu-id="47075-110">Crie uma instância da `SimpleProvider` classe passando uma função que retornará um token de acesso para escopos aprovados.</span><span class="sxs-lookup"><span data-stu-id="47075-110">Instantiate the `SimpleProvider` class by passing in a function that will return an access token for passed-in scopes.</span></span> 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

<span data-ttu-id="47075-111">Além disso, você também pode fornecer uma `login` função opcional e `logout` que possa lidar com as chamadas de entrada e de saída do componente de [logon](../components/login.md) .</span><span class="sxs-lookup"><span data-stu-id="47075-111">In addition, you can also provide an optional `login` and `logout` functions that can handle the sign in and sign out calls from the [Login](../components/login.md) component.</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="47075-112">Para indicar aos componentes que eles podem começar a chamar as APIs do Microsoft Graph após um usuário entrar com êxito, você precisará chamar `Providers.setState(ProviderState.SignedIn)` .</span><span class="sxs-lookup"><span data-stu-id="47075-112">To indicate to the components that they can start calling the Microsoft Graph APIs after a user successfully signs in, you need to call `Providers.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="47075-113">Um exemplo disso é mostrado na função a `login` seguir.</span><span class="sxs-lookup"><span data-stu-id="47075-113">An example of this is shown in the `login` function below.</span></span>

```ts
function getAccessToken(scopes: string[]) {
  // return a promise with accessToken string
}

function login() {
  //login code
  Providers.globalProvider.setState(ProviderState.SignedIn)
}

function logout() {
  // logout code
}

let provider = new SimpleProvider(getAccessToken, login, logout);
```

### <a name="manage-state"></a><span data-ttu-id="47075-114">Gerenciar estado</span><span class="sxs-lookup"><span data-stu-id="47075-114">Manage state</span></span>

<span data-ttu-id="47075-115">Para que os componentes estejam cientes do estado do provedor, será necessário chamar o `provider.setState(state: ProviderState)` método sempre que o estado for alterado.</span><span class="sxs-lookup"><span data-stu-id="47075-115">For the components to be aware of the state of the provider, you will need to call the `provider.setState(state: ProviderState)` method whenever the state changes.</span></span> <span data-ttu-id="47075-116">Por exemplo, quando o usuário entrou, ligue para `provider.setState(ProviderState.SignedIn)` .</span><span class="sxs-lookup"><span data-stu-id="47075-116">For example, when the user has signed in, call `provider.setState(ProviderState.SignedIn)`.</span></span> <span data-ttu-id="47075-117">A `ProviderState` enumeração define três Estados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="47075-117">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a><span data-ttu-id="47075-118">IProvider</span><span class="sxs-lookup"><span data-stu-id="47075-118">IProvider</span></span>

<span data-ttu-id="47075-119">Você pode estender a `IProvider` classe abstract para criar seu próprio provedor.</span><span class="sxs-lookup"><span data-stu-id="47075-119">You can extend the `IProvider` abstract class to create your own provider.</span></span>

### <a name="state"></a><span data-ttu-id="47075-120">Estado</span><span class="sxs-lookup"><span data-stu-id="47075-120">State</span></span>

<span data-ttu-id="47075-121">Um provedor deve acompanhar o estado de autenticação e atualizar os componentes quando o estado for alterado.</span><span class="sxs-lookup"><span data-stu-id="47075-121">A provider must keep track of the authentication state and update the components when the state changes.</span></span> <span data-ttu-id="47075-122">A `IProvider` classe já implementa o `onStateChanged(eventHandler)` manipulador e a `state: ProviderState` propriedade.</span><span class="sxs-lookup"><span data-stu-id="47075-122">The `IProvider` class already implements the `onStateChanged(eventHandler)` handler and the `state: ProviderState` property.</span></span> <span data-ttu-id="47075-123">Você só precisa usar o `setState(state:ProviderState)` método na sua implementação para atualizar o estado quando ele for alterado.</span><span class="sxs-lookup"><span data-stu-id="47075-123">You just need to use the `setState(state:ProviderState)` method in your implementation to update the state when it changes.</span></span> <span data-ttu-id="47075-124">A atualização do estado acionará o `stateChanged` evento e atualizará todos os componentes automaticamente.</span><span class="sxs-lookup"><span data-stu-id="47075-124">Updating the state will fire the `stateChanged` event and update all the components automatically.</span></span>

### <a name="loginlogout"></a><span data-ttu-id="47075-125">Login/logout</span><span class="sxs-lookup"><span data-stu-id="47075-125">Login/Logout</span></span>

<span data-ttu-id="47075-126">Se seu provedor fornece a funcionalidade de logon ou logout, implemente os `login(): Promise<void>` `logout(): Promise<void>` métodos e.</span><span class="sxs-lookup"><span data-stu-id="47075-126">If your provider provides login or logout functionality, implement the `login(): Promise<void>` and `logout(): Promise<void>` methods.</span></span> <span data-ttu-id="47075-127">Esses métodos são opcionais.</span><span class="sxs-lookup"><span data-stu-id="47075-127">These methods are optional.</span></span>

### <a name="access-token"></a><span data-ttu-id="47075-128">Token de acesso</span><span class="sxs-lookup"><span data-stu-id="47075-128">Access token</span></span>

<span data-ttu-id="47075-129">Você deve implementar o `getAccessToken({'scopes': scopes[]}) : Promise<string>` método.</span><span class="sxs-lookup"><span data-stu-id="47075-129">You must implement the `getAccessToken({'scopes': scopes[]}) : Promise<string>` method.</span></span> <span data-ttu-id="47075-130">Este método é usado para obter um token válido antes de cada chamada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47075-130">This method is used to get a valid token before every call to Microsoft Graph.</span></span>

### <a name="graph"></a><span data-ttu-id="47075-131">Graph</span><span class="sxs-lookup"><span data-stu-id="47075-131">Graph</span></span>

<span data-ttu-id="47075-132">Os componentes usam o SDK do JavaScript do Microsoft Graph para todas as chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47075-132">The components use the Microsoft Graph Javascript SDK for all calls to Microsoft Graph.</span></span> <span data-ttu-id="47075-133">Seu provedor deve tornar o SDK disponível por meio da `graph` propriedade.</span><span class="sxs-lookup"><span data-stu-id="47075-133">Your provider must make the SDK available through the `graph` property.</span></span> <span data-ttu-id="47075-134">No construtor, crie uma nova `Graph` instância, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="47075-134">In your constructor, create a new `Graph` instance, as shown.</span></span>

```js
this.graph = new Graph(this);
```

<span data-ttu-id="47075-135">A `Graph` classe é um invólucro claro na parte superior do SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47075-135">The `Graph` class is a light wrapper on top of the Microsoft Graph SDK.</span></span>

### <a name="example"></a><span data-ttu-id="47075-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47075-136">Example</span></span>

<span data-ttu-id="47075-137">Todos os provedores estendem a `IProvider` classe abstrata.</span><span class="sxs-lookup"><span data-stu-id="47075-137">All the providers extend the `IProvider` abstract class.</span></span> <span data-ttu-id="47075-138">Para obter exemplos, dê uma olhada no código-fonte de qualquer um dos [provedores existentes](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span><span class="sxs-lookup"><span data-stu-id="47075-138">For examples, take a look at the source code for any of the [existing providers](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).</span></span>

## <a name="set-the-global-provider"></a><span data-ttu-id="47075-139">Definir o provedor global</span><span class="sxs-lookup"><span data-stu-id="47075-139">Set the global provider</span></span>

<span data-ttu-id="47075-140">Os componentes usam a `Providers.globalProvider` propriedade para acessar um provedor.</span><span class="sxs-lookup"><span data-stu-id="47075-140">Components use the `Providers.globalProvider` property to access a provider.</span></span> <span data-ttu-id="47075-141">Depois de criar seu próprio provedor, defina essa propriedade como seu provedor.</span><span class="sxs-lookup"><span data-stu-id="47075-141">After you create your own provider, set this property to your provider.</span></span>

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

<span data-ttu-id="47075-142">Todos os componentes serão notificados do novo provedor e começarão a usá-lo.</span><span class="sxs-lookup"><span data-stu-id="47075-142">All the components will be notified of the new provider and start using it.</span></span>
