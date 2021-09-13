---
title: Provedor personalizado
description: Crie um provedor personalizado para habilitar a autenticação e o acesso gráfico para os componentes do Microsoft Graph Toolkit, se você tiver código de autenticação existente em seu aplicativo.
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: be470ed25acccb3fcdd1499b0048a33dae7c5d13
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143557"
---
# <a name="custom-provider"></a>Provedor personalizado

Se você tiver código de autenticação existente em seu aplicativo, poderá criar um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph para componentes Graph Toolkit Microsoft. Há duas maneiras de criar provedores personalizados:

- Criar um novo `SimpleProvider` passando uma função para obter um token de acesso
- Estender a `IProvider` classe abstrata

Este artigo descreve cada abordagem com mais detalhes.

## <a name="simpleprovider"></a>SimpleProvider

Insinue a classe passando uma função que retornará um `SimpleProvider` token de acesso para escopos passados. 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

Além disso, você também pode fornecer um opcional e funções que podem manipular a entrar e fazer chamadas `login` `logout` do componente De [logon.](../components/login.md)

> [!IMPORTANT] 
> Para indicar aos componentes que eles podem começar a chamar as APIs do Microsoft Graph depois que um usuário entrar com êxito, você precisa chamar `Providers.setState(ProviderState.SignedIn)` . Um exemplo disso é mostrado na `login` função abaixo.

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

### <a name="manage-state"></a>Gerenciar estado

Para que os componentes sejam cientes do estado do provedor, você precisará chamar o método sempre `provider.setState(state: ProviderState)` que o estado mudar. Por exemplo, quando o usuário tiver se assinado, chame `provider.setState(ProviderState.SignedIn)` . O `ProviderState` número define três estados, conforme mostrado.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

Você pode estender a `IProvider` classe abstrata para criar seu próprio provedor.

### <a name="state"></a>Estado

Um provedor deve acompanhar o estado de autenticação e atualizar os componentes quando o estado mudar. A `IProvider` classe já implementa o manipulador e a `onStateChanged(eventHandler)` `state: ProviderState` propriedade. Você só precisa usar o `setState(state:ProviderState)` método em sua implementação para atualizar o estado quando ele mudar. A atualização do estado disparará o `stateChanged` evento e atualizará todos os componentes automaticamente.

### <a name="loginlogout"></a>Logout/Logout

Se o provedor fornece funcionalidade de logon ou logout, implemente `login(): Promise<void>` os `logout(): Promise<void>` métodos e. Esses métodos são opcionais.

### <a name="access-token"></a>Token de acesso

Você deve implementar o `getAccessToken({'scopes': scopes[]}) : Promise<string>` método. Esse método é usado para obter um token válido antes de cada chamada para o Microsoft Graph.

### <a name="graph"></a>Graph

Os componentes usam o Microsoft Graph Javascript SDK para todas as chamadas para o Microsoft Graph. Seu provedor deve disponibilizar o SDK por meio da `graph` propriedade. Em seu construtor, crie uma nova `Graph` instância, conforme mostrado.

```js
this.graph = new Graph(this);
```

A `Graph` classe é um invólucro claro sobre o Microsoft Graph SDK.

### <a name="example"></a>Exemplo

Todos os provedores estendem a `IProvider` classe abstrata. Por exemplo, dê uma olhada no código-fonte de qualquer um dos [provedores existentes.](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/mgt/src/providers)

## <a name="set-the-global-provider"></a>Definir o provedor global

Os componentes usam `Providers.globalProvider` a propriedade para acessar um provedor. Depois de criar seu próprio provedor, de definir essa propriedade como seu provedor.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Todos os componentes serão notificados do novo provedor e começarão a usá-lo.
