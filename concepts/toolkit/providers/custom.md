---
title: Provedor personalizado
description: Crie um provedor personalizado para habilitar a autenticação e o acesso de gráfico para os componentes do Microsoft Graph Toolkit, se você tiver um código de autenticação existente em seu aplicativo.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4e287a38a584f77b7dfedf6e36d56da7a4e29715
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643733"
---
# <a name="custom-provider"></a>Provedor personalizado

Se você tiver um código de autenticação existente em seu aplicativo, poderá criar um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph para os componentes do Microsoft Graph Toolkit. Há duas maneiras de criar provedores personalizados:

- Criar um novo `SimpleProvider` passando uma função para obter um token de acesso
- Estender a `IProvider` classe abstrata

Este artigo descreve cada abordagem em mais detalhes.

## <a name="simpleprovider"></a>Simpleprovider

Crie uma instância da `SimpleProvider` classe passando uma função que retornará um token de acesso para escopos aprovados.

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

Além disso, você também pode fornecer uma `login` função opcional e `logout` que possa lidar com as chamadas de entrada e de saída do componente de [logon](../components/login.md) .

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

### <a name="manage-state"></a>Gerenciar estado

Para que os componentes estejam cientes do estado do provedor, será necessário chamar o `provider.setState(state: ProviderState)` método sempre que o estado for alterado. Por exemplo, quando o usuário entrou, ligue para `provider.setState(ProviderState.SignedIn)` . A `ProviderState` enumeração define três Estados, conforme mostrado.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

Você pode estender a `IProvider` classe abstract para criar seu próprio provedor.

### <a name="state"></a>State

Um provedor deve acompanhar o estado de autenticação e atualizar os componentes quando o estado for alterado. A `IProvider` classe já implementa o `onStateChanged(eventHandler)` manipulador e a `state: ProviderState` propriedade. Você só precisa usar o `setState(state:ProviderState)` método na sua implementação para atualizar o estado quando ele for alterado. A atualização do estado acionará o `stateChanged` evento e atualizará todos os componentes automaticamente.

### <a name="loginlogout"></a>Login/logout

Se seu provedor fornece a funcionalidade de logon ou logout, implemente os `login(): Promise<void>` `logout(): Promise<void>` métodos e. Esses métodos são opcionais.

### <a name="access-token"></a>Token de acesso

Você deve implementar o `getAccessToken({'scopes': scopes[]}) : Promise<string>` método. Este método é usado para obter um token válido antes de cada chamada para o Microsoft Graph.

### <a name="graph"></a>Graph

Os componentes usam o SDK do JavaScript do Microsoft Graph para todas as chamadas para o Microsoft Graph. Seu provedor deve tornar o SDK disponível por meio da `graph` propriedade. No construtor, crie uma nova `Graph` instância, conforme mostrado.

```js
this.graph = new Graph(this);
```

A `Graph` classe é um invólucro claro na parte superior do SDK do Microsoft Graph.

### <a name="example"></a>Exemplo

Todos os provedores estendem a `IProvider` classe abstrata. Para obter exemplos, dê uma olhada no código-fonte de qualquer um dos [provedores existentes](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers).

## <a name="set-the-global-provider"></a>Definir o provedor global

Os componentes usam a `Providers.globalProvider` propriedade para acessar um provedor. Depois de criar seu próprio provedor, defina essa propriedade como seu provedor.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Todos os componentes serão notificados do novo provedor e começarão a usá-lo.
