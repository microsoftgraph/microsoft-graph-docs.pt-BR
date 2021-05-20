---
title: Microsoft Graph Toolkit provedores
description: Os provedores Graph Toolkit Microsoft habilitam a autenticação e o microsoft Graph acesso para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 05cbd59758b27266db7444333c72a2ba3a766ebb
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579694"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="a239c-103">Microsoft Graph Toolkit provedores</span><span class="sxs-lookup"><span data-stu-id="a239c-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="a239c-104">Os provedores Graph Toolkit Microsoft permitem que seu aplicativo se autenture com a Microsoft Identity e acesse o Microsoft Graph em apenas algumas linhas de código.</span><span class="sxs-lookup"><span data-stu-id="a239c-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="a239c-105">Cada provedor lida com a autenticação do usuário e a aquisição dos tokens de acesso para chamar as APIs do Microsoft Graph, para que você não tenha que escrever esse código por conta própria.</span><span class="sxs-lookup"><span data-stu-id="a239c-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="a239c-106">Você pode usar os provedores por conta própria, sem componentes, para implementar rapidamente a autenticação para seu aplicativo e fazer chamadas para a Microsoft Graph por meio do SDK do cliente JavaScript.</span><span class="sxs-lookup"><span data-stu-id="a239c-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="a239c-107">Os provedores são necessários ao usar os componentes do Microsoft Graph Toolkit como os componentes os usam para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a239c-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="a239c-108">Se você já tiver sua própria autenticação e quiser usar os componentes, poderá usar um [provedor personalizado.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="a239c-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="a239c-109">O Toolkit inclui os seguintes provedores.</span><span class="sxs-lookup"><span data-stu-id="a239c-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="a239c-110">Provedores</span><span class="sxs-lookup"><span data-stu-id="a239c-110">Providers</span></span>|<span data-ttu-id="a239c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a239c-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="a239c-112">Msal</span><span class="sxs-lookup"><span data-stu-id="a239c-112">Msal</span></span>](./msal.md)|<span data-ttu-id="a239c-113">Usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="a239c-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="a239c-114">Msal 2.0</span><span class="sxs-lookup"><span data-stu-id="a239c-114">Msal 2.0</span></span>](./msal2.md)| <span data-ttu-id="a239c-115">Usa o msal-browser para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="a239c-115">Uses msal-browser to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span> | 
|[<span data-ttu-id="a239c-116">Tron</span><span class="sxs-lookup"><span data-stu-id="a239c-116">Electron</span></span>](./electron.md)|<span data-ttu-id="a239c-117">Autentica e fornece à Microsoft Graph acesso a componentes dentro dos aplicativos Detron.</span><span class="sxs-lookup"><span data-stu-id="a239c-117">Authenticates and provides Microsoft Graph access to components inside of Electron apps.</span></span>|
|[<span data-ttu-id="a239c-118">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a239c-118">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="a239c-119">Autentica e fornece à Microsoft Graph acesso a componentes dentro de SharePoint Web Parts.</span><span class="sxs-lookup"><span data-stu-id="a239c-119">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="a239c-120">Teams</span><span class="sxs-lookup"><span data-stu-id="a239c-120">Teams</span></span>](./teams.md)|<span data-ttu-id="a239c-121">Autentica e fornece à Microsoft Graph acesso a componentes dentro Microsoft Teams guias.</span><span class="sxs-lookup"><span data-stu-id="a239c-121">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="a239c-122">Proxy</span><span class="sxs-lookup"><span data-stu-id="a239c-122">Proxy</span></span>](./proxy.md)|<span data-ttu-id="a239c-123">Permite o uso da autenticação de back-end roteamento de todas as chamadas para a Microsoft Graph seu back-end.</span><span class="sxs-lookup"><span data-stu-id="a239c-123">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="a239c-124">Personalizados</span><span class="sxs-lookup"><span data-stu-id="a239c-124">Custom</span></span>](./custom.md)|<span data-ttu-id="a239c-125">Crie um provedor personalizado para habilitar a autenticação e o acesso à Microsoft Graph com o código de autenticação existente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a239c-125">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="a239c-126">Inicializando um provedor</span><span class="sxs-lookup"><span data-stu-id="a239c-126">Initializing a provider</span></span>

<span data-ttu-id="a239c-127">Para usar um provedor em seu aplicativo, você precisa inicializar um novo provedor e defini-lo como o provedor global no namespace Provedores.</span><span class="sxs-lookup"><span data-stu-id="a239c-127">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="a239c-128">Recomendamos fazer isso antes de começar a usar qualquer um dos componentes.</span><span class="sxs-lookup"><span data-stu-id="a239c-128">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="a239c-129">Você pode fazer isso de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="a239c-129">You can do this one of two ways:</span></span>

<span data-ttu-id="a239c-130">**Opção 1: Usar o componente do provedor**</span><span class="sxs-lookup"><span data-stu-id="a239c-130">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="a239c-131">Você pode usar a versão do componente do provedor diretamente em seu HTML.</span><span class="sxs-lookup"><span data-stu-id="a239c-131">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="a239c-132">Nos bastidores, um novo provedor é inicializado e definido como o provedor global.</span><span class="sxs-lookup"><span data-stu-id="a239c-132">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="a239c-133">O exemplo a seguir mostra como usar o Msal2Provider.</span><span class="sxs-lookup"><span data-stu-id="a239c-133">The following example shows how to use the Msal2Provider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
```

<span data-ttu-id="a239c-134">**Opção 2: Inicializar no código**</span><span class="sxs-lookup"><span data-stu-id="a239c-134">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="a239c-135">Inicializar seu provedor em seu código JavaScript permite que você forneça mais opções.</span><span class="sxs-lookup"><span data-stu-id="a239c-135">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="a239c-136">Para fazer isso, crie uma nova instância de provedor e de definir o valor da propriedade para o `Providers.globalProvider` provedor que você gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="a239c-136">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="a239c-137">O exemplo a seguir mostra como usar o Msal2Provider.</span><span class="sxs-lookup"><span data-stu-id="a239c-137">The following example shows how to use the Msal2Provider.</span></span>

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="a239c-138">**Observação:** Para obter detalhes sobre como registrar seu aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="a239c-138">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="a239c-139">Escopos de permissão</span><span class="sxs-lookup"><span data-stu-id="a239c-139">Permission Scopes</span></span>

<span data-ttu-id="a239c-140">Recomendamos adicionar todos os escopos de permissão que seu aplicativo precisa ao atributo ou propriedade ao inicializar seu provedor (isso não se aplica ao provedor `scopes` [SharePoint ).](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="a239c-140">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="a239c-141">Isso é opcional, mas melhorará a experiência do usuário apresentando uma única tela de consentimento para o usuário com uma lista agregada de permissões solicitadas por todos os componentes em seu aplicativo, em vez de apresentar telas separadas para cada componente.</span><span class="sxs-lookup"><span data-stu-id="a239c-141">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="a239c-142">Os exemplos a seguir mostram como fazer isso com o Msal2Provider.</span><span class="sxs-lookup"><span data-stu-id="a239c-142">The following examples show how to do this with the Msal2Provider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal2-provider>
```

<span data-ttu-id="a239c-143">Se você estiver inicializando o provedor em código, forneça os escopos de permissão em uma matriz na `scopes` propriedade.</span><span class="sxs-lookup"><span data-stu-id="a239c-143">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, Msal2Provider } from "@microsoft/mgt";
Providers.globalProvider = new Msal2Provider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="a239c-144">Você pode encontrar a lista de escopos de permissão exigidos por cada componente na seção Permissões do **Microsoft Graph** da página de documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="a239c-144">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="a239c-145">Estado do provedor</span><span class="sxs-lookup"><span data-stu-id="a239c-145">Provider state</span></span>

<span data-ttu-id="a239c-146">O provedor mantém o controle do estado de autenticação do usuário e o comunica aos componentes.</span><span class="sxs-lookup"><span data-stu-id="a239c-146">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="a239c-147">Por exemplo, quando um usuário faz a entrada com êxito, o é atualizado para , sinalizando para os componentes que agora são capazes de fazer chamadas para o `ProviderState` `SignedIn` Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a239c-147">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="a239c-148">O `ProviderState` número define três estados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="a239c-148">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="a239c-149">Em alguns cenários, você vai querer mostrar determinada funcionalidade ou executar uma ação somente depois que um usuário tiver se assinado com êxito.</span><span class="sxs-lookup"><span data-stu-id="a239c-149">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="a239c-150">Você pode acessar e verificar o estado do provedor, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a239c-150">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="a239c-151">Você também pode usar o `Providers.onProviderUpdated` método para ser notificado sempre que o estado do provedor mudar.</span><span class="sxs-lookup"><span data-stu-id="a239c-151">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

const providerStateChanged = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    // user is now signed in
  }
}

// register a callback for when the state changes
Providers.onProviderUpdated(providerStateChanged);

// remove callback if necessary
Providers.removeProviderUpdatedListener(providerStateChanged);
```

## <a name="getting-an-access-token"></a><span data-ttu-id="a239c-152">Obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="a239c-152">Getting an access token</span></span>

<span data-ttu-id="a239c-153">Cada provedor expõe uma função chamada que pode recuperar o token de acesso atual ou recuperar um novo token de `getAccessToken` acesso para os escopos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="a239c-153">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="a239c-154">O exemplo a seguir mostra como obter um novo token de acesso com o `User.Read` escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="a239c-154">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = await Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="a239c-155">Fazendo suas próprias chamadas para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a239c-155">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="a239c-156">Todos os componentes podem acessar o Microsoft Graph sem qualquer personalização necessária desde que você inicialize um provedor (conforme descrito nas seções anteriores).</span><span class="sxs-lookup"><span data-stu-id="a239c-156">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="a239c-157">Se você quiser fazer suas próprias chamadas para o Microsoft Graph, faça isso recebendo uma referência ao mesmo SDK do Microsoft Graph usado pelos componentes.</span><span class="sxs-lookup"><span data-stu-id="a239c-157">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="a239c-158">Primeiro, obter uma referência para o global `IProvider` e, em seguida, usar o `graph` objeto conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="a239c-158">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="a239c-159">Pode haver casos em que você precisa passar permissões adicionais, dependendo da API que você está chamando.</span><span class="sxs-lookup"><span data-stu-id="a239c-159">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="a239c-160">O exemplo a seguir mostra como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="a239c-160">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="a239c-161">Usando vários provedores</span><span class="sxs-lookup"><span data-stu-id="a239c-161">Using multiple providers</span></span>

<span data-ttu-id="a239c-162">Em alguns cenários, seu aplicativo será executado em ambientes diferentes e exigirá um provedor diferente para cada um.</span><span class="sxs-lookup"><span data-stu-id="a239c-162">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="a239c-163">Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia Microsoft Teams, o que significa que você pode precisar usar o Msal2Provider e o TeamsProvider.</span><span class="sxs-lookup"><span data-stu-id="a239c-163">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the Msal2Provider and the TeamsProvider.</span></span> <span data-ttu-id="a239c-164">Para esse cenário, todos os componentes do provedor têm o atributo para criar uma cadeia `depends-on` de fallback, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a239c-164">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal2-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal2-provider>
```

<span data-ttu-id="a239c-165">Nesse cenário, o Msal2Provider só será usado se seu aplicativo estiver sendo executado como um aplicativo Web e o TeamsProvider não estiver disponível no ambiente atual.</span><span class="sxs-lookup"><span data-stu-id="a239c-165">In this scenario, the Msal2Provider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="a239c-166">Para fazer o mesmo no código, você pode usar a `isAvailable` propriedade no provedor, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="a239c-166">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new Msal2Provider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="a239c-167">Logout/Logout do Usuário</span><span class="sxs-lookup"><span data-stu-id="a239c-167">User Login/Logout</span></span>

<span data-ttu-id="a239c-168">Quando você tem os provedores corretos inicializados para seu aplicativo, você pode adicionar o componente [de Logon](../components/login.md) do Toolkit para implementar logon e logout do usuário de forma fácil e rápida.</span><span class="sxs-lookup"><span data-stu-id="a239c-168">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="a239c-169">O componente funciona com o provedor para lidar com toda a lógica de autenticação e a funcionalidade de logout/logout.</span><span class="sxs-lookup"><span data-stu-id="a239c-169">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="a239c-170">O exemplo a seguir usa o Msal2Provider e o componente Logon.</span><span class="sxs-lookup"><span data-stu-id="a239c-170">The following example uses the Msal2Provider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="YOUR_CLIENT_ID"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="a239c-171">Em cenários em que você deseja implementar isso por conta própria, em vez de usar o componente de Logon do Toolkit, você pode fazer isso usando os métodos e `login` `logout` do provedor.</span><span class="sxs-lookup"><span data-stu-id="a239c-171">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="a239c-172">Implementar seu próprio provedor</span><span class="sxs-lookup"><span data-stu-id="a239c-172">Implement your own provider</span></span>

<span data-ttu-id="a239c-173">Em cenários em que você deseja adicionar Toolkit componentes a um aplicativo com código de autenticação pré-existente, você pode criar um provedor personalizado que se ligue ao mecanismo de autenticação, em vez de usar nossos provedores predefinidos.</span><span class="sxs-lookup"><span data-stu-id="a239c-173">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="a239c-174">O kit de ferramentas fornece duas maneiras de criar novos provedores:</span><span class="sxs-lookup"><span data-stu-id="a239c-174">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="a239c-175">Crie um novo que retorna um token de acesso do código de `SimpleProvider` autenticação passando uma função.</span><span class="sxs-lookup"><span data-stu-id="a239c-175">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="a239c-176">Estender a `IProvider` classe abstrata.</span><span class="sxs-lookup"><span data-stu-id="a239c-176">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="a239c-177">Para obter mais detalhes sobre cada um, consulte [provedores personalizados.](../providers/custom.md)</span><span class="sxs-lookup"><span data-stu-id="a239c-177">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
