---
title: Provedores de kit de ferramentas do Microsoft Graph
description: Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4b51fdf91fd37c0c3dc5ea0ec49571a8ed4e5d47
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086644"
---
# <a name="microsoft-graph-toolkit-providers"></a><span data-ttu-id="fd785-103">Provedores de kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fd785-103">Microsoft Graph Toolkit providers</span></span>

<span data-ttu-id="fd785-104">Os provedores do Microsoft Graph Toolkit permitem que seu aplicativo seja autenticado com a identidade da Microsoft e acesse o Microsoft Graph somente em algumas linhas de código.</span><span class="sxs-lookup"><span data-stu-id="fd785-104">The Microsoft Graph Toolkit providers enable your application to authenticate with Microsoft Identity and access Microsoft Graph in only few lines of code.</span></span> <span data-ttu-id="fd785-105">Cada provedor trata a autenticação do usuário e a aquisição dos tokens de acesso para chamar as APIs do Microsoft Graph, para que você não precise escrever esse código por conta própria.</span><span class="sxs-lookup"><span data-stu-id="fd785-105">Each provider handles user authentication and acquiring the access tokens to call Microsoft Graph APIs, so that you don't have to write this code yourself.</span></span> 

<span data-ttu-id="fd785-106">Você pode usar os provedores sozinhos, sem componentes, para implementar rapidamente a autenticação para seu aplicativo e fazer chamadas para o Microsoft Graph por meio do SDK do cliente JavaScript.</span><span class="sxs-lookup"><span data-stu-id="fd785-106">You can use the providers on their own, without components, to quickly implement authentication for your app and make calls to Microsoft Graph via the JavaScript client SDK.</span></span>

<span data-ttu-id="fd785-107">Os provedores são necessários ao usar os componentes do Microsoft Graph Toolkit à medida que os componentes os usam para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd785-107">The providers are required when using the Microsoft Graph Toolkit components as the components use them to access Microsoft Graph.</span></span> <span data-ttu-id="fd785-108">Se você já tiver sua própria autenticação e quiser usar os componentes, poderá usar um [provedor personalizado](./providers/custom.md) .</span><span class="sxs-lookup"><span data-stu-id="fd785-108">If you already have your own authentication and want to use the components, you can use a [custom provider](./providers/custom.md) instead.</span></span>

<span data-ttu-id="fd785-109">O kit de ferramentas inclui os provedores a seguir.</span><span class="sxs-lookup"><span data-stu-id="fd785-109">The Toolkit includes the following providers.</span></span>

|<span data-ttu-id="fd785-110">Provedores</span><span class="sxs-lookup"><span data-stu-id="fd785-110">Providers</span></span>|<span data-ttu-id="fd785-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd785-111">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="fd785-112">MSAL</span><span class="sxs-lookup"><span data-stu-id="fd785-112">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="fd785-113">Usa MSAL.js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph em um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="fd785-113">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph in a web application.</span></span>|
|[<span data-ttu-id="fd785-114">SharePoint</span><span class="sxs-lookup"><span data-stu-id="fd785-114">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="fd785-115">Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fd785-115">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="fd785-116">Teams</span><span class="sxs-lookup"><span data-stu-id="fd785-116">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="fd785-117">Autentica e fornece acesso do Microsoft Graph aos componentes dentro de guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fd785-117">Authenticates and provides Microsoft Graph access to components inside  Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="fd785-118">Acionista</span><span class="sxs-lookup"><span data-stu-id="fd785-118">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="fd785-119">Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.</span><span class="sxs-lookup"><span data-stu-id="fd785-119">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="fd785-120">Personalizados</span><span class="sxs-lookup"><span data-stu-id="fd785-120">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="fd785-121">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd785-121">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="initializing-a-provider"></a><span data-ttu-id="fd785-122">Inicializando um provedor</span><span class="sxs-lookup"><span data-stu-id="fd785-122">Initializing a provider</span></span>

<span data-ttu-id="fd785-123">Para usar um provedor em seu aplicativo, você precisa inicializar um novo provedor e, em seguida, defini-lo como o provedor global no namespace de provedores.</span><span class="sxs-lookup"><span data-stu-id="fd785-123">To use a provider in your app, you need to initialize a new provider and then set it as the global provider in the Providers namespace.</span></span> <span data-ttu-id="fd785-124">É recomendável fazer isso antes de começar a usar qualquer um dos componentes.</span><span class="sxs-lookup"><span data-stu-id="fd785-124">We recommend doing this before you start using any of the components.</span></span> <span data-ttu-id="fd785-125">Você pode fazer isso de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="fd785-125">You can do this one of two ways:</span></span>

<span data-ttu-id="fd785-126">**Opção 1: usar o componente do provedor**</span><span class="sxs-lookup"><span data-stu-id="fd785-126">**Option 1: Use the provider component**</span></span>

<span data-ttu-id="fd785-127">Você pode usar a versão do componente do provedor diretamente no HTML.</span><span class="sxs-lookup"><span data-stu-id="fd785-127">You can use the component version of the provider directly in your HTML.</span></span> <span data-ttu-id="fd785-128">Nos bastidores, um novo provedor é inicializado e definido como o provedor global.</span><span class="sxs-lookup"><span data-stu-id="fd785-128">Behind the scenes, a new provider is initialized and set as the global provider.</span></span> <span data-ttu-id="fd785-129">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="fd785-129">The following example shows how to use the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

<span data-ttu-id="fd785-130">**Opção 2: inicializar no código**</span><span class="sxs-lookup"><span data-stu-id="fd785-130">**Option 2: Initialize in code**</span></span>

<span data-ttu-id="fd785-131">Inicializar seu provedor em seu código JavaScript permite que você forneça mais opções.</span><span class="sxs-lookup"><span data-stu-id="fd785-131">Initializing your provider in your JavaScript code enables you to provide more options.</span></span> <span data-ttu-id="fd785-132">Para fazer isso, crie uma nova instância de provedor e defina o valor da `Providers.globalProvider` propriedade para o provedor que você gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="fd785-132">To do this, create a new provider instance and set the value of the `Providers.globalProvider` property to the provider you'd like to use.</span></span> <span data-ttu-id="fd785-133">O exemplo a seguir mostra como usar o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="fd785-133">The following example shows how to use the MsalProvider.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> <span data-ttu-id="fd785-134">**Observação:** Para obter detalhes sobre como registrar seu aplicativo e obter uma ID de cliente, consulte [criar um aplicativo do Azure Active Directory](./get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="fd785-134">**Note:** For details about how to register your app and get a client ID, see [Create an Azure Active Directory app](./get-started/add-aad-app-registration.md).</span></span>

## <a name="permission-scopes"></a><span data-ttu-id="fd785-135">Escopos de permissão</span><span class="sxs-lookup"><span data-stu-id="fd785-135">Permission Scopes</span></span>

<span data-ttu-id="fd785-136">Recomendamos adicionar todos os escopos de permissão que seu aplicativo precisa ao `scopes` atributo ou à propriedade ao inicializar o provedor (isso não se aplica ao [provedor do SharePoint](./providers/sharepoint.md)).</span><span class="sxs-lookup"><span data-stu-id="fd785-136">We recommend adding all the permission scopes your application needs to the `scopes` attribute or property when initializing your provider (this does not apply to the [SharePoint provider](./providers/sharepoint.md)).</span></span> <span data-ttu-id="fd785-137">Isso é opcional, mas melhorará a experiência do usuário apresentando uma única tela de consentimento para o usuário com uma lista agregada de permissões solicitadas por todos os componentes em seu aplicativo, em vez de apresentar telas separadas para cada componente.</span><span class="sxs-lookup"><span data-stu-id="fd785-137">This is optional, but will improve your user experience by presenting a single consent screen to the user with an aggregated list of permissions requested by all components in your app, rather than presenting separate screens for each component.</span></span> <span data-ttu-id="fd785-138">Os exemplos a seguir mostram como fazer isso com o MsalProvider.</span><span class="sxs-lookup"><span data-stu-id="fd785-138">The following examples show how to do this with the MsalProvider.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

<span data-ttu-id="fd785-139">Se você estiver inicializando o provedor no código, forneça os escopos de permissão em uma matriz na `scopes` propriedade.</span><span class="sxs-lookup"><span data-stu-id="fd785-139">If you're initializing the provider in code, provide the permission scopes in an array in the `scopes` property.</span></span>

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

<span data-ttu-id="fd785-140">Você pode encontrar a lista de escopos de permissão exigido por cada componente na seção **permissões do Microsoft Graph** da página de documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="fd785-140">You can find the list of permission scopes required by each component in the **Microsoft Graph permissions** section of each component's documentation page.</span></span>

## <a name="provider-state"></a><span data-ttu-id="fd785-141">Estado do provedor</span><span class="sxs-lookup"><span data-stu-id="fd785-141">Provider state</span></span>

<span data-ttu-id="fd785-142">O provedor mantém o controle do estado de autenticação do usuário e o comunica com os componentes.</span><span class="sxs-lookup"><span data-stu-id="fd785-142">The provider keeps track of the user's authentication state and communicates it to the components.</span></span> <span data-ttu-id="fd785-143">Por exemplo, quando um usuário faz o logon com êxito, o `ProviderState` é atualizado para `SignedIn` , sinalizando para os componentes que agora eles podem fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fd785-143">For example, when a user successfully signs in, the `ProviderState` is updated to `SignedIn`, signaling to the components that they are now able to make calls to Microsoft Graph.</span></span> <span data-ttu-id="fd785-144">A `ProviderState` enumeração define três Estados, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="fd785-144">The `ProviderState` enum defines three states, as shown.</span></span>

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

<span data-ttu-id="fd785-145">Em alguns cenários, você vai querer mostrar determinada funcionalidade ou executar uma ação somente após um usuário ter entrado com êxito.</span><span class="sxs-lookup"><span data-stu-id="fd785-145">In some scenarios, you will want to show certain functionality or perform an action only after a user has successfully signed in.</span></span> <span data-ttu-id="fd785-146">Você pode acessar e verificar o estado do provedor, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="fd785-146">You can access and check the provider state, as shown in the following example.</span></span>

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
<span data-ttu-id="fd785-147">Você também pode usar o `Providers.onProviderUpdated` método para ser notificado sempre que o estado do provedor for alterado.</span><span class="sxs-lookup"><span data-stu-id="fd785-147">You can also use the `Providers.onProviderUpdated` method to get notified whenever the state of the provider changes.</span></span>

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

## <a name="getting-an-access-token"></a><span data-ttu-id="fd785-148">Como obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="fd785-148">Getting an access token</span></span>

<span data-ttu-id="fd785-149">Cada provedor expõe uma função chamada `getAccessToken` que pode recuperar o token de acesso atual ou recuperar um novo token de acesso para os escopos fornecidos.</span><span class="sxs-lookup"><span data-stu-id="fd785-149">Each provider exposes a function called `getAccessToken` that can retreive the current access token or retrieve a new access token for the provided scopes.</span></span> <span data-ttu-id="fd785-150">O exemplo a seguir mostra como obter um novo token de acesso com o `User.Read` escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="fd785-150">The following example shows how to get a new access token with the `User.Read` permission scope.</span></span>

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Provider.globalProvider.getAccessToken({scopes: 'User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a><span data-ttu-id="fd785-151">Fazendo suas próprias chamadas para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fd785-151">Making your own calls to Microsoft Graph</span></span>

<span data-ttu-id="fd785-152">Todos os componentes podem acessar o Microsoft Graph sem qualquer personalização necessária, desde que você inicialize um provedor (conforme descrito nas seções anteriores).</span><span class="sxs-lookup"><span data-stu-id="fd785-152">All components can access Microsoft Graph without any customization required as long as you initialize a provider (as described in the previous sections).</span></span> <span data-ttu-id="fd785-153">Se quiser fazer suas próprias chamadas para o Microsoft Graph, você pode fazer isso obtendo uma referência para o mesmo SDK do Microsoft Graph usado pelos componentes.</span><span class="sxs-lookup"><span data-stu-id="fd785-153">If you want to make your own calls to Microsoft Graph, you can do so by getting a reference to the same Microsoft Graph SDK used by the components.</span></span> <span data-ttu-id="fd785-154">Primeiro, obtenha uma referência para o global `IProvider` e use o `graph` objeto conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="fd785-154">First, get a reference to the global `IProvider` and then use the `graph` object as shown:</span></span>

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
<span data-ttu-id="fd785-155">Pode haver casos em que você precisa passar permissões adicionais, dependendo da API que você está chamando.</span><span class="sxs-lookup"><span data-stu-id="fd785-155">There might be cases where you need to pass additional permissions, depending on the API you're calling.</span></span> <span data-ttu-id="fd785-156">O exemplo a seguir mostra como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="fd785-156">The following example shows how to do this.</span></span>

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a><span data-ttu-id="fd785-157">Usando vários provedores</span><span class="sxs-lookup"><span data-stu-id="fd785-157">Using multiple providers</span></span>

<span data-ttu-id="fd785-158">Em alguns cenários, o aplicativo será executado em diferentes ambientes e exigirá um provedor diferente para cada um.</span><span class="sxs-lookup"><span data-stu-id="fd785-158">In some scenarios, your application will run in different environments and require a different provider for each.</span></span> <span data-ttu-id="fd785-159">Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, o que significa que você pode precisar usar o MsalProvider e o Teamprovider.</span><span class="sxs-lookup"><span data-stu-id="fd785-159">For example, the app might run as both a web application and a Microsoft Teams tab, which means you might need to use both the MsalProvider and the TeamsProvider.</span></span> <span data-ttu-id="fd785-160">Para este cenário, todos os componentes do provedor têm o `depends-on` atributo para criar uma cadeia de fallback, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="fd785-160">For this scenario, all provider components have the `depends-on` attribute to create a fallback chain, as shown in the following example.</span></span>

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

<span data-ttu-id="fd785-161">Neste cenário, o MsalProvider será usado somente se seu aplicativo estiver sendo executado como um aplicativo Web e o Teams não estiver disponível no ambiente atual.</span><span class="sxs-lookup"><span data-stu-id="fd785-161">In this scenario, the MsalProvider will only be used if your app is running as a web application and the TeamsProvider is not available in the current environment.</span></span>

<span data-ttu-id="fd785-162">Para fazer o mesmo no código, você pode usar a `isAvailable` propriedade no provedor, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="fd785-162">To accomplish the same in code, you can use the `isAvailable` property on the provider, as shown.</span></span>

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a><span data-ttu-id="fd785-163">Login/logoff de usuário</span><span class="sxs-lookup"><span data-stu-id="fd785-163">User Login/Logout</span></span>

<span data-ttu-id="fd785-164">Quando você tem os provedores adequados inicializados para seu aplicativo, você pode adicionar o [componente de login](./components/login.md) do kit de ferramentas para implementar de forma fácil e rápida o login e o logoff do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd785-164">When you have the right providers initialized for your application, you can add the Toolkit's [Login component](./components/login.md) to easily and quickly implement user login and logout.</span></span> <span data-ttu-id="fd785-165">O componente funciona com o provedor para lidar com toda a lógica de autenticação e a funcionalidade de logon/logout.</span><span class="sxs-lookup"><span data-stu-id="fd785-165">The component works with the provider to handle all of the authentication logic and login/logout functionality.</span></span> <span data-ttu-id="fd785-166">O exemplo a seguir usa o MsalProvider e o componente de logon.</span><span class="sxs-lookup"><span data-stu-id="fd785-166">The following example uses the MsalProvider and the Login component.</span></span>

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

<span data-ttu-id="fd785-167">Em cenários em que você deseja implementar isso sozinho, em vez de usar o componente de login do kit de ferramentas, você pode fazer isso usando os `login` `logout` métodos e do provedor.</span><span class="sxs-lookup"><span data-stu-id="fd785-167">In scenarios where you want to implement this yourself, rather than using the Toolkit's Login component, you can do so by using the `login` and `logout` methods of the provider.</span></span>

## <a name="implement-your-own-provider"></a><span data-ttu-id="fd785-168">Implementar seu próprio provedor</span><span class="sxs-lookup"><span data-stu-id="fd785-168">Implement your own provider</span></span>

<span data-ttu-id="fd785-169">Em cenários em que você deseja adicionar componentes de kit de ferramentas a um aplicativo com código de autenticação pré-existente, você pode criar um provedor personalizado que se conecta ao seu mecanismo de autenticação, em vez de usar nossos provedores predefinidos.</span><span class="sxs-lookup"><span data-stu-id="fd785-169">In scenarios where you want to add Toolkit components to an application with pre-existing authentication code, you can create a custom provider that hooks into your authentication mechanism, instead of using our predefined providers.</span></span> <span data-ttu-id="fd785-170">O kit de ferramentas fornece duas maneiras de criar novos provedores:</span><span class="sxs-lookup"><span data-stu-id="fd785-170">The toolkit provides two ways to create new providers:</span></span>

- <span data-ttu-id="fd785-171">Crie um novo `SimpleProvider` que retorne um token de acesso do seu código de autenticação passando uma função.</span><span class="sxs-lookup"><span data-stu-id="fd785-171">Create a new `SimpleProvider` that returns an access token from your authentication code by passing in a function.</span></span>
- <span data-ttu-id="fd785-172">Estenda a `IProvider` classe abstract.</span><span class="sxs-lookup"><span data-stu-id="fd785-172">Extend the `IProvider` abstract class.</span></span>

<span data-ttu-id="fd785-173">Para obter mais detalhes sobre cada um, consulte [Custom Providers](./providers/custom.md).</span><span class="sxs-lookup"><span data-stu-id="fd785-173">For more details about each one, see [custom providers](./providers/custom.md).</span></span>
