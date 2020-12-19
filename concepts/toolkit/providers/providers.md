---
title: Provedores de kit de ferramentas do Microsoft Graph
description: Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e130e6d56123f847d9c92e16de0e0449c208c7b6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720018"
---
# <a name="microsoft-graph-toolkit-providers"></a>Provedores de kit de ferramentas do Microsoft Graph

Os provedores do Microsoft Graph Toolkit permitem que seu aplicativo seja autenticado com a identidade da Microsoft e acesse o Microsoft Graph somente em algumas linhas de código. Cada provedor trata a autenticação do usuário e a aquisição dos tokens de acesso para chamar as APIs do Microsoft Graph, para que você não precise escrever esse código por conta própria. 

Você pode usar os provedores sozinhos, sem componentes, para implementar rapidamente a autenticação para seu aplicativo e fazer chamadas para o Microsoft Graph por meio do SDK do cliente JavaScript.

Os provedores são necessários ao usar os componentes do Microsoft Graph Toolkit à medida que os componentes os usam para acessar o Microsoft Graph. Se você já tiver sua própria autenticação e quiser usar os componentes, poderá usar um [provedor personalizado](./custom.md) .

O kit de ferramentas inclui os provedores a seguir.

|Provedores|Descrição|
|---------|-----------|
|[MSAL](./msal.md)|Usa MSAL.js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph em um aplicativo Web.|
|[SharePoint](./sharepoint.md)|Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.|
|[Teams](./teams.md)|Autentica e fornece acesso do Microsoft Graph aos componentes dentro de guias do Microsoft Teams.|
|[Acionista](./proxy.md)|Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.|
|[Personalizados](./custom.md)|Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.|

## <a name="initializing-a-provider"></a>Inicializando um provedor

Para usar um provedor em seu aplicativo, você precisa inicializar um novo provedor e, em seguida, defini-lo como o provedor global no namespace de provedores. É recomendável fazer isso antes de começar a usar qualquer um dos componentes. Você pode fazer isso de duas maneiras:

**Opção 1: usar o componente do provedor**

Você pode usar a versão do componente do provedor diretamente no HTML. Nos bastidores, um novo provedor é inicializado e definido como o provedor global. O exemplo a seguir mostra como usar o MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
```

**Opção 2: inicializar no código**

Inicializar seu provedor em seu código JavaScript permite que você forneça mais opções. Para fazer isso, crie uma nova instância de provedor e defina o valor da `Providers.globalProvider` propriedade para o provedor que você gostaria de usar. O exemplo a seguir mostra como usar o MsalProvider.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
});
```
> **Observação:** Para obter detalhes sobre como registrar seu aplicativo e obter uma ID de cliente, consulte [criar um aplicativo do Azure Active Directory](../get-started/add-aad-app-registration.md).

## <a name="permission-scopes"></a>Escopos de permissão

Recomendamos adicionar todos os escopos de permissão que seu aplicativo precisa ao `scopes` atributo ou à propriedade ao inicializar o provedor (isso não se aplica ao [provedor do SharePoint](../providers/sharepoint.md)). Isso é opcional, mas melhorará a experiência do usuário apresentando uma única tela de consentimento para o usuário com uma lista agregada de permissões solicitadas por todos os componentes em seu aplicativo, em vez de apresentar telas separadas para cada componente. Os exemplos a seguir mostram como fazer isso com o MsalProvider.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"
                   scopes="user.read,people.read"
                   ></mgt-msal-provider>
```

Se você estiver inicializando o provedor no código, forneça os escopos de permissão em uma matriz na `scopes` propriedade.

```js
import {Providers, MsalProvider } from "@microsoft/mgt";
Providers.globalProvider = new MsalProvider({
  clientId: 'YOUR_CLIENT_ID'
  scopes:['user.read','people.read']
});
```

Você pode encontrar a lista de escopos de permissão exigido por cada componente na seção **permissões do Microsoft Graph** da página de documentação de cada componente.

## <a name="provider-state"></a>Estado do provedor

O provedor mantém o controle do estado de autenticação do usuário e o comunica com os componentes. Por exemplo, quando um usuário faz o logon com êxito, o `ProviderState` é atualizado para `SignedIn` , sinalizando para os componentes que agora eles podem fazer chamadas para o Microsoft Graph. A `ProviderState` enumeração define três Estados, conforme mostrado.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

Em alguns cenários, você vai querer mostrar determinada funcionalidade ou executar uma ação somente após um usuário ter entrado com êxito. Você pode acessar e verificar o estado do provedor, conforme mostrado no exemplo a seguir.

```js
import { Providers, ProviderState } from '@microsoft/mgt'

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  //your code here
}
```
Você também pode usar o `Providers.onProviderUpdated` método para ser notificado sempre que o estado do provedor for alterado.

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

Cada provedor expõe uma função chamada `getAccessToken` que pode recuperar o token de acesso atual ou recuperar um novo token de acesso para os escopos fornecidos. O exemplo a seguir mostra como obter um novo token de acesso com o `User.Read` escopo de permissão.

```js
import { Providers, ProviderState } from "@microsoft/mgt";

//assuming a provider has already been initialized

if (Providers.globalProvider.state === ProviderState.SignedIn) {
  const token = Providers.globalProvider.getAccessToken({scopes: ['User.Read']})
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Fazendo suas próprias chamadas para o Microsoft Graph

Todos os componentes podem acessar o Microsoft Graph sem qualquer personalização necessária, desde que você inicialize um provedor (conforme descrito nas seções anteriores). Se quiser fazer suas próprias chamadas para o Microsoft Graph, você pode fazer isso obtendo uma referência para o mesmo SDK do Microsoft Graph usado pelos componentes. Primeiro, obtenha uma referência para o global `IProvider` e use o `graph` objeto conforme mostrado:

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

Em alguns cenários, o aplicativo será executado em diferentes ambientes e exigirá um provedor diferente para cada um. Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, o que significa que você pode precisar usar o MsalProvider e o Teamprovider. Para este cenário, todos os componentes do provedor têm o `depends-on` atributo para criar uma cadeia de fallback, conforme mostrado no exemplo a seguir.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

Neste cenário, o MsalProvider será usado somente se seu aplicativo estiver sendo executado como um aplicativo Web e o Teams não estiver disponível no ambiente atual.

Para fazer o mesmo no código, você pode usar a `isAvailable` propriedade no provedor, conforme mostrado.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```
## <a name="user-loginlogout"></a>Login/logoff de usuário

Quando você tem os provedores adequados inicializados para seu aplicativo, você pode adicionar o [componente de login](../components/login.md) do kit de ferramentas para implementar de forma fácil e rápida o login e o logoff do usuário. O componente funciona com o provedor para lidar com toda a lógica de autenticação e a funcionalidade de logon/logout. O exemplo a seguir usa o MsalProvider e o componente de logon.

```HTML
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="YOUR_CLIENT_ID"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Em cenários em que você deseja implementar isso sozinho, em vez de usar o componente de login do kit de ferramentas, você pode fazer isso usando os `login` `logout` métodos e do provedor.

## <a name="implement-your-own-provider"></a>Implementar seu próprio provedor

Em cenários em que você deseja adicionar componentes de kit de ferramentas a um aplicativo com código de autenticação pré-existente, você pode criar um provedor personalizado que se conecta ao seu mecanismo de autenticação, em vez de usar nossos provedores predefinidos. O kit de ferramentas fornece duas maneiras de criar novos provedores:

- Crie um novo `SimpleProvider` que retorne um token de acesso do seu código de autenticação passando uma função.
- Estenda a `IProvider` classe abstract.

Para obter mais detalhes sobre cada um, consulte [Custom Providers](../providers/custom.md).
