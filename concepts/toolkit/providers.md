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
# <a name="microsoft-graph-toolkit-providers"></a>Provedores de kit de ferramentas do Microsoft Graph

Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para todos os componentes. Cada provedor fornece uma implementação para adquirir o token de acesso necessário para chamar as APIs do Microsoft Graph.

Para que os componentes usem um provedor, você deve definir a `Providers.globalProvider` Propriedade como o valor de um provedor que você gostaria de usar.

O exemplo a seguir mostra como usar o MsalProvider.

```js
Providers.globalProvider = new MsalProvider({
  clientId: '[CLIENT_ID]'
});
```

O kit de ferramentas implementa os seguintes provedores:

- [MsalProvider](./providers/msal.md)
- [SharePointprovider](./providers/sharepoint.md)
- [Teamprovider](./providers/teams.md)
- Provedor de suplementos do Office (em breve)

## <a name="get-started"></a>Introdução

Você pode criar um provedor a qualquer momento. Recomendamos que você crie o provedor antes de usar qualquer um dos componentes. Esta seção descreve como inicializar um provedor.

A `Providers` variável global expõe as seguintes propriedades e funções

- `globalProvider : IProvider`

Defina essa propriedade como um provedor que você deseja usar globalmente. Todos os componentes usam essa propriedade para obter uma referência ao provedor. A definição dessa propriedade acionará `onProvidersChanged` o evento.

- `function onProviderUpdated(callbackFunction)`

A `callbackFunction` função será chamada quando um provedor for alterado ou quando o estado de um provedor for alterado. Um `ProvidersChangedState` valor de enumeração será passado para a função para indicar o que foi atualizado.

## <a name="implement-your-own-provider"></a>Implementar seu próprio provedor

O kit de ferramentas fornece duas maneiras de criar novos provedores:

- Criar um novo `SimpleProvider` passando uma função para obter um token de acesso
- Estender a `IProvider` classe abstrata

Leia mais sobre cada um na documentação dos [provedores personalizados](./providers/custom.md) .

## <a name="using-multiple-providers"></a>Usando vários provedores

Em alguns cenários, seu aplicativo será executado em um ambiente diferente e exigirá um provedor diferente. Por exemplo, o aplicativo pode ser executado como um aplicativo Web e uma guia do Microsoft Teams, e você pode precisar usar o MsalProvider e o Teamprovider. Para este cenário, todos os componentes do provedor `depends-on` têm o atributo para criar uma cadeia de fallback, conforme mostrado no exemplo a seguir.

```html
<mgt-teams-provider
  client-id="[CLIENT-ID]"
  auth-popup-url="auth.html" ></mgt-teams-provider>

<mgt-msal-provider
  client-id="[CLIENT-ID]"
  depends-on="mgt-teams-provider" ></mgt-msal-provider>
```

Neste cenário, o MsalProvider será usado somente se o Teams não estiver disponível no ambiente atual.

Para fazer o mesmo no código, você pode usar a `isAvailable` Propriedade no provedor, conforme mostrado.

```ts
if (TeamsProvider.isAvailable) {
    Providers.globalProvider = new TeamsProvider(teamsConfig);
} else {
    Providers.globalProvider = new MsalProvider(msalConfig)
}
```

## <a name="making-your-own-calls-to-microsoft-graph"></a>Fazendo suas próprias chamadas para o Microsoft Graph

Todos os componentes podem acessar o Microsoft Graph sem a necessidade de personalização, desde que você inicialize um provedor (conforme descrito na seção anterior). Para obter uma referência para o mesmo SDK do Microsoft Graph usado pelos componentes, primeiro obtenha uma referência para o IProvider global e, em seguida `Graph` , use o objeto, conforme mostrado.

```js
import { Providers } from '@microsoft/mgt';

let provider = Providers.globalProvider;
if (provider) {
  let graphClient = provider.graph.client;
  let userDetails = await graphClient.api('me').get();
}
```

Pode haver casos em que você precisará transmitir permissões adicionais, dependendo da API que você está chamando.

```js
import { prepScopes } from '@microsoft/mgt';

graphClient
  .api('me')
  .middlewareOptions(prepScopes('user.read', 'calendar.read'))
  .get();
```

O `graph` objeto é uma instância do [SDK do JavaScript do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) e você pode usá-lo para fazer chamadas para o Microsoft Graph.
