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
# <a name="microsoft-graph-toolkit-providers"></a>Microsoft Graph Toolkit provedores

Os provedores de Toolkit do Microsoft Graph permitem que seu aplicativo se autenture com a Microsoft Identity e acesse o Microsoft Graph em apenas algumas linhas de código. Cada provedor lida com a autenticação do usuário e a aquisição dos tokens de acesso para chamar APIs do Microsoft Graph, para que você não tenha que escrever esse código por conta própria. 

Você pode usar os provedores por conta própria, sem componentes, para implementar rapidamente a autenticação para seu aplicativo e fazer chamadas para o Microsoft Graph por meio do SDK do cliente JavaScript.

Os provedores são necessários ao usar os componentes do Microsoft Graph Toolkit como os componentes os usam para acessar o Microsoft Graph. Se você já tiver sua própria autenticação e quiser usar os componentes, poderá usar um [provedor personalizado.](./custom.md)

O Toolkit inclui os seguintes provedores.

|Provedores|Descrição|
|---------|-----------|
|[Msal](./msal.md)|Usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Web.|
|[Tron](./electron.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro dos aplicativos Dols.|
|[SharePoint](./sharepoint.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro das Web Parts do SharePoint.|
|[Teams](./teams.md)|Autentica e fornece acesso do Microsoft Graph a componentes dentro das guias do Microsoft Teams.|
|[Proxy](./proxy.md)|Permite o uso da autenticação de back-end roteamento de todas as chamadas para o Microsoft Graph por meio do back-end.|
|[Personalizados](./custom.md)|Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do aplicativo.|

## <a name="initializing-a-provider"></a>Inicializando um provedor

Para usar um provedor em seu aplicativo, você precisa inicializar um novo provedor e defini-lo como o provedor global no namespace Provedores. Recomendamos fazer isso antes de começar a usar qualquer um dos componentes. Você pode fazer isso de duas maneiras:

**Opção 1: Usar o componente do provedor**

Você pode usar a versão do componente do provedor diretamente em seu HTML. Nos bastidores, um novo provedor é inicializado e definido como o provedor global. O exemplo a seguir mostra como usar o MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**Opção 2: Inicializar no código**

Inicializar seu provedor em seu código JavaScript permite que você forneça mais opções. Para fazer isso, crie uma nova instância de provedor e de definir o valor da propriedade para o `Providers.globalProvider` provedor que você gostaria de usar. O exemplo a seguir mostra como usar o MsalProvider.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Observação:** Para obter detalhes sobre como registrar seu aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).

## <a name="permission-scopes"></a>Escopos de permissão

Recomendamos adicionar todos os escopos de permissão que seu aplicativo precisa ao atributo ou propriedade ao inicializar seu provedor (isso não se aplica `scopes` ao provedor [do SharePoint](../providers/sharepoint.md)). Isso é opcional, mas melhorará a experiência do usuário apresentando uma única tela de consentimento para o usuário com uma lista agregada de permissões solicitadas por todos os componentes em seu aplicativo, em vez de apresentar telas separadas para cada componente. Os exemplos a seguir mostram como fazer isso com o MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

Se você estiver inicializando o provedor em código, forneça os escopos de permissão em uma matriz na `scopes` propriedade.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Você pode encontrar a lista de escopos de permissão exigidos por cada componente na seção permissões do **Microsoft Graph** da página de documentação de cada componente.

## <a name="provider-state"></a>Estado do provedor

O provedor mantém o controle do estado de autenticação do usuário e o comunica aos componentes. Por exemplo, quando um usuário faz entrada com êxito, o é atualizado para , sinalizando para os componentes que agora são capazes de fazer chamadas `ProviderState` `SignedIn` para o Microsoft Graph. O `ProviderState` número define três estados, conforme mostrado.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

Em alguns cenários, você vai querer mostrar determinada funcionalidade ou executar uma ação somente depois que um usuário tiver se assinado com êxito. Você pode acessar e verificar o estado do provedor, conforme mostrado no exemplo a seguir.

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
Você também pode usar o `Providers.onProviderUpdated` método para ser notificado sempre que o estado do provedor mudar.

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

## <a name="getting-an-access-token"></a>Como obter um token de acesso

Cada provedor expõe uma função chamada que pode recuperar o token de acesso atual ou recuperar um novo token de `getAccessToken` acesso para os escopos fornecidos. O exemplo a seguir mostra como obter um novo token de acesso com o `User.Read` escopo de permissão.

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Fazendo suas próprias chamadas para o Microsoft Graph

Todos os componentes podem acessar o Microsoft Graph sem qualquer personalização necessária desde que você inicialize um provedor (conforme descrito nas seções anteriores). Se quiser fazer suas próprias chamadas para o Microsoft Graph, faça isso fazendo referência ao mesmo SDK do Microsoft Graph usado pelos componentes. Primeiro, obter uma referência para o global `IProvider` e, em seguida, usar o `graph` objeto conforme mostrado:

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```
Pode haver casos em que você precisa passar permissões adicionais, dependendo da API que você está chamando. O exemplo a seguir mostra como fazer isso.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

## <a name="using-multiple-providers"></a>Usando vários provedores

Em alguns cenários, seu aplicativo será executado em ambientes diferentes e exigirá um provedor diferente para cada um. Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, o que significa que talvez seja necessário usar o MsalProvider e o TeamsProvider. Para esse cenário, todos os componentes do provedor têm o atributo para criar uma cadeia `depends-on` de fallback, conforme mostrado no exemplo a seguir.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

Nesse cenário, o MsalProvider só será usado se seu aplicativo estiver sendo executado como um aplicativo Web e o TeamsProvider não estiver disponível no ambiente atual.

Para fazer o mesmo no código, você pode usar a `isAvailable` propriedade no provedor, conforme mostrado.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Logout/Logout do Usuário

Quando você tem os provedores corretos inicializados para seu aplicativo, você pode adicionar o componente [de Logon](../components/login.md) do Toolkit para implementar logon e logout do usuário de forma fácil e rápida. O componente funciona com o provedor para lidar com toda a lógica de autenticação e a funcionalidade de logout/logout. O exemplo a seguir usa o MsalProvider e o componente Logon.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Em cenários em que você deseja implementar isso por conta própria, em vez de usar o componente de Logon do Toolkit, você pode fazer isso usando os métodos e `login` `logout` do provedor.

## <a name="implement-your-own-provider"></a>Implementar seu próprio provedor

Em cenários em que você deseja adicionar Toolkit componentes a um aplicativo com código de autenticação pré-existente, você pode criar um provedor personalizado que se ligue ao mecanismo de autenticação, em vez de usar nossos provedores predefinidos. O kit de ferramentas fornece duas maneiras de criar novos provedores:

- Crie um novo que retorna um token de acesso do código de `SimpleProvider` autenticação passando uma função.
- Estender a `IProvider` classe abstrata.

Para obter mais detalhes sobre cada um, consulte [provedores personalizados.](../providers/custom.md)
