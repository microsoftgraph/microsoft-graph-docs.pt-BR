---
title: Microsoft Graph Toolkit provedores
description: Os provedores de Toolkit do Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c6fa59632464d0cfa801b07a30d6a5cf94ae5c76
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470281"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="4bb5f-103">Microsoft Graph Toolkit provedores</span><span class="sxs-lookup"><span data-stu-id="4bb5f-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="4bb5f-104">Os provedores de Toolkit do Microsoft Graph permitem que seu aplicativo se autenture com a Microsoft Identity e acesse o Microsoft Graph em apenas algumas linhas de código.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="4bb5f-105">Cada provedor lida com a autenticação do usuário e a aquisição dos tokens de acesso para chamar APIs do Microsoft Graph, para que você não tenha que escrever esse código por conta própria.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="4bb5f-106">Você pode usar os provedores por conta própria, sem componentes, para implementar rapidamente a autenticação para seu aplicativo e fazer chamadas para o Microsoft Graph por meio do SDK do cliente JavaScript.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="4bb5f-107">Os provedores são necessários ao usar os componentes do Microsoft Graph Toolkit como os componentes os usam para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="4bb5f-108">Se você já tiver sua própria autenticação e quiser usar os componentes, poderá usar um [provedor personalizado.](./custom.md)</span><span class="sxs-lookup"><span data-stu-id="4bb5f-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./custom.md) instead.</span></span>

<span data-ttu-id="4bb5f-109">O Toolkit inclui os seguintes provedores.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="4bb5f-110">Provedores</span><span class="sxs-lookup"><span data-stu-id="4bb5f-110">Providers</span></span>|<span data-ttu-id="4bb5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bb5f-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="4bb5f-112">Msal</span><span class="sxs-lookup"><span data-stu-id="4bb5f-112">Msal</span></span>](./msal.md)|<span data-ttu-id="4bb5f-113">Usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="4bb5f-114">Tron</span><span class="sxs-lookup"><span data-stu-id="4bb5f-114">Electron</span></span>](./electron.md)|<span data-ttu-id="4bb5f-115">Autentica e fornece acesso do Microsoft Graph a componentes dentro dos aplicativos Dols.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-115">Authenticates and provides Microsoft Graph access to components inside of Electron apps.</span></span>|
|[<span data-ttu-id="4bb5f-116">SharePoint</span><span class="sxs-lookup"><span data-stu-id="4bb5f-116">SharePoint</span></span>](./sharepoint.md)|<span data-ttu-id="4bb5f-117">Autentica e fornece acesso do Microsoft Graph a componentes dentro das Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-117">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="4bb5f-118">Teams</span><span class="sxs-lookup"><span data-stu-id="4bb5f-118">Teams</span></span>](./teams.md)|<span data-ttu-id="4bb5f-119">Autentica e fornece acesso do Microsoft Graph a componentes dentro das guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-119">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="4bb5f-120">Proxy</span><span class="sxs-lookup"><span data-stu-id="4bb5f-120">Proxy</span></span>](./proxy.md)|<span data-ttu-id="4bb5f-121">Permite o uso da autenticação de back-end roteamento de todas as chamadas para o Microsoft Graph por meio do back-end.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-121">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="4bb5f-122">Personalizados</span><span class="sxs-lookup"><span data-stu-id="4bb5f-122">Custom</span></span>](./custom.md)|<span data-ttu-id="4bb5f-123">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-123">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="4bb5f-124">Inicializando um provedor</span><span class="sxs-lookup"><span data-stu-id="4bb5f-124">Initializing a provider</span></span>

<span data-ttu-id="4bb5f-125">Para usar um provedor em seu aplicativo, você precisa inicializar um novo provedor e defini-lo como o provedor global no namespace Provedores.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-125">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="4bb5f-126">Recomendamos fazer isso antes de começar a usar qualquer um dos componentes.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-126">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="4bb5f-127">Você pode fazer isso de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="4bb5f-127">You can do this one of two ways:</span></span>

<span data-ttu-id="4bb5f-128">**Opção 1: Usar o componente do provedor**</span><span class="sxs-lookup"><span data-stu-id="4bb5f-128">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="4bb5f-129">Você pode usar a versão do componente do provedor diretamente em seu HTML.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-129">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="4bb5f-130">Nos bastidores, um novo provedor é inicializado e definido como o provedor global.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-130">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="4bb5f-131">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-131">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="4bb5f-132">**Opção 2: Inicializar no código**</span><span class="sxs-lookup"><span data-stu-id="4bb5f-132">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="4bb5f-133">Inicializar seu provedor em seu código JavaScript permite que você forneça mais opções.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-133">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="4bb5f-134">Para fazer isso, crie uma nova instância de provedor e de definir o valor da propriedade para o `Providers.globalProvider` provedor que você gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-134">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="4bb5f-135">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-135">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="4bb5f-136">**Observação:** Para obter detalhes sobre como registrar seu aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="4bb5f-136">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="4bb5f-137">Escopos de permissão</span><span class="sxs-lookup"><span data-stu-id="4bb5f-137">Permission Scopes</span></span>

<span data-ttu-id="4bb5f-138">Recomendamos adicionar todos os escopos de permissão que seu aplicativo precisa ao atributo ou propriedade ao inicializar seu provedor (isso não se aplica `scopes` ao provedor [do SharePoint](../providers/sharepoint.md)).</span><span class="sxs-lookup"><span data-stu-id="4bb5f-138">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](../providers/sharepoint.md)).</span></span> <span data-ttu-id="4bb5f-139">Isso é opcional, mas melhorará a experiência do usuário apresentando uma única tela de consentimento para o usuário com uma lista agregada de permissões solicitadas por todos os componentes em seu aplicativo, em vez de apresentar telas separadas para cada componente.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-139">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="4bb5f-140">Os exemplos a seguir mostram como fazer isso com o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-140">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="4bb5f-141">Se você estiver inicializando o provedor em código, forneça os escopos de permissão em uma matriz na `scopes` propriedade.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-141">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="4bb5f-142">Você pode encontrar a lista de escopos de permissão exigidos por cada componente na seção permissões do **Microsoft Graph** da página de documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-142">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="4bb5f-143">Estado do provedor</span><span class="sxs-lookup"><span data-stu-id="4bb5f-143">Provider state</span></span>

<span data-ttu-id="4bb5f-144">O provedor mantém o controle do estado de autenticação do usuário e o comunica aos componentes.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-144">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="4bb5f-145">Por exemplo, quando um usuário faz entrada com êxito, o é atualizado para , sinalizando para os componentes que agora são capazes de fazer chamadas `ProviderState` `SignedIn` para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-145">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="4bb5f-146">O `ProviderState` número define três estados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-146">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="4bb5f-147">Em alguns cenários, você vai querer mostrar determinada funcionalidade ou executar uma ação somente depois que um usuário tiver se assinado com êxito.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-147">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="4bb5f-148">Você pode acessar e verificar o estado do provedor, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-148">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="4bb5f-149">Você também pode usar o `Providers.onProviderUpdated` método para ser notificado sempre que o estado do provedor mudar.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-149">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

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

## <a name="getting-an-access-token"></a><span data-ttu-id="4bb5f-150">Como obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="4bb5f-150">Getting an access token</span></span>

<span data-ttu-id="4bb5f-151">Cada provedor expõe uma função chamada que pode recuperar o token de acesso atual ou recuperar um novo token de `getAccessToken` acesso para os escopos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-151">Each provider exposes a function called `getAccessToken` that can retrieve the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="4bb5f-152">O exemplo a seguir mostra como obter um novo token de acesso com o `User.Read` escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-152">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="4bb5f-153">Fazendo suas próprias chamadas para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4bb5f-153">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="4bb5f-154">Todos os componentes podem acessar o Microsoft Graph sem qualquer personalização necessária desde que você inicialize um provedor (conforme descrito nas seções anteriores).</span><span class="sxs-lookup"><span data-stu-id="4bb5f-154">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="4bb5f-155">Se quiser fazer suas próprias chamadas para o Microsoft Graph, faça isso fazendo referência ao mesmo SDK do Microsoft Graph usado pelos componentes.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-155">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="4bb5f-156">Primeiro, obter uma referência para o global `IProvider` e, em seguida, usar o `graph` objeto conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="4bb5f-156">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="4bb5f-157">Pode haver casos em que você precisa passar permissões adicionais, dependendo da API que você está chamando.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-157">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="4bb5f-158">O exemplo a seguir mostra como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-158">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="4bb5f-159">Usando vários provedores</span><span class="sxs-lookup"><span data-stu-id="4bb5f-159">Using multiple providers</span></span>

<span data-ttu-id="4bb5f-160">Em alguns cenários, seu aplicativo será executado em ambientes diferentes e exigirá um provedor diferente para cada um.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-160">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="4bb5f-161">Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, o que significa que talvez seja necessário usar o MsalProvider e o TeamsProvider.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-161">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="4bb5f-162">Para esse cenário, todos os componentes do provedor têm o atributo para criar uma cadeia `depends-on` de fallback, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-162">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="4bb5f-163">Nesse cenário, o MsalProvider só será usado se seu aplicativo estiver sendo executado como um aplicativo Web e o TeamsProvider não estiver disponível no ambiente atual.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-163">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="4bb5f-164">Para fazer o mesmo no código, você pode usar a `isAvailable` propriedade no provedor, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-164">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="4bb5f-165">Logout/Logout do Usuário</span><span class="sxs-lookup"><span data-stu-id="4bb5f-165">User Login/Logout</span></span>

<span data-ttu-id="4bb5f-166">Quando você tem os provedores corretos inicializados para seu aplicativo, você pode adicionar o componente [de Logon](../components/login.md) do Toolkit para implementar logon e logout do usuário de forma fácil e rápida.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-166">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](../components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="4bb5f-167">O componente funciona com o provedor para lidar com toda a lógica de autenticação e a funcionalidade de logout/logout.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-167">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="4bb5f-168">O exemplo a seguir usa o MsalProvider e o componente Logon.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-168">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="4bb5f-169">Em cenários em que você deseja implementar isso por conta própria, em vez de usar o componente de Logon do Toolkit, você pode fazer isso usando os métodos e `login` `logout` do provedor.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-169">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="4bb5f-170">Implementar seu próprio provedor</span><span class="sxs-lookup"><span data-stu-id="4bb5f-170">Implement your own provider</span></span>

<span data-ttu-id="4bb5f-171">Em cenários em que você deseja adicionar Toolkit componentes a um aplicativo com código de autenticação pré-existente, você pode criar um provedor personalizado que se ligue ao mecanismo de autenticação, em vez de usar nossos provedores predefinidos.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-171">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="4bb5f-172">O kit de ferramentas fornece duas maneiras de criar novos provedores:</span><span class="sxs-lookup"><span data-stu-id="4bb5f-172">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="4bb5f-173">Crie um novo que retorna um token de acesso do código de `SimpleProvider` autenticação passando uma função.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-173">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="4bb5f-174">Estender a `IProvider` classe abstrata.</span><span class="sxs-lookup"><span data-stu-id="4bb5f-174">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="4bb5f-175">Para obter mais detalhes sobre cada um, consulte [provedores personalizados.](../providers/custom.md)</span><span class="sxs-lookup"><span data-stu-id="4bb5f-175">For more details about each one, see [custom providers](../providers/custom.md).</span></span>
