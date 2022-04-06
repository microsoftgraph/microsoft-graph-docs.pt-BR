---
title: Provedor personalizado
description: Crie um provedor personalizado para habilitar a autenticação e o acesso gráfico para os componentes do Microsoft Graph Toolkit, se você tiver código de autenticação existente em seu aplicativo.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 2373c30a37e761d1cd14b203aa07edfc80eecfad
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589300"
---
# <a name="custom-provider"></a>Provedor personalizado

Se você tiver código de autenticação existente em seu aplicativo, poderá criar um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph para componentes do Microsoft Graph Toolkit. Há duas maneiras de criar provedores personalizados:

- Criar um novo `SimpleProvider` passando uma função para obter um token de acesso
- Estender a classe `IProvider` abstrata

Este artigo descreve cada abordagem com mais detalhes.

## <a name="simpleprovider"></a>SimpleProvider

Insinue `SimpleProvider` a classe passando uma função que retornará um token de acesso para escopos passados. 

```ts
let provider = new SimpleProvider((scopes: string[]) => {
  // return a promise with accessToken
});
```

Além disso, você também pode fornecer um opcional `login` `logout` e funções que podem manipular a entrar e fazer chamadas do [componente De logon](../components/login.md) .

> [!IMPORTANT] 
> Para indicar aos componentes que eles podem começar a chamar as APIs do Microsoft Graph depois que um usuário entrar com êxito, você precisa chamar `Providers.setState(ProviderState.SignedIn)`. Um exemplo disso é mostrado na função `login` abaixo.

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

Para que os componentes sejam cientes do estado do provedor, você precisará chamar o `provider.setState(state: ProviderState)` método sempre que o estado mudar. Por exemplo, quando o usuário tiver se assinado, chame `provider.setState(ProviderState.SignedIn)`. O `ProviderState` número define três estados, conforme mostrado.

```ts
export enum ProviderState {
  Loading,
  SignedOut,
  SignedIn
}
```

## <a name="iprovider"></a>IProvider

Você pode estender a classe `IProvider` abstrata para criar seu próprio provedor.

### <a name="state"></a>Estado

Um provedor deve acompanhar o estado de autenticação e atualizar os componentes quando o estado mudar. A `IProvider` classe já implementa o manipulador `onStateChanged(eventHandler)` e a `state: ProviderState` propriedade. Você só precisa usar o método `setState(state:ProviderState)` em sua implementação para atualizar o estado quando ele mudar. A atualização do estado disparará o evento `stateChanged` e atualizará todos os componentes automaticamente.

### <a name="loginlogout"></a>Logout/Logout

Se o provedor fornece funcionalidade de logon ou logout, implemente os `login(): Promise<void>` métodos e `logout(): Promise<void>` . Esses métodos são opcionais.

### <a name="access-token"></a>Token de acesso

Você deve implementar o `getAccessToken({'scopes': scopes[]}) : Promise<string>` método. Esse método é usado para obter um token válido antes de cada chamada para o Microsoft Graph.

### <a name="graph"></a>Graph

Os componentes usam o Microsoft Graph Javascript SDK para todas as chamadas para o Microsoft Graph. Seu provedor deve disponibilizar o SDK por meio da `graph` propriedade. Em seu construtor, crie uma nova `Graph` instância, conforme mostrado.

```js
this.graph = new Graph(this);
```

A `Graph` classe é um invólucro claro na parte superior do Microsoft Graph SDK.

### <a name="example"></a>Exemplo

Todos os provedores estendem a classe `IProvider` abstrata. Por exemplo, dê uma olhada no código-fonte de qualquer um dos [provedores existentes](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/packages/providers).

## <a name="set-the-global-provider"></a>Definir o provedor global

Os componentes usam `Providers.globalProvider` a propriedade para acessar um provedor. Depois de criar seu próprio provedor, de definir essa propriedade como seu provedor.

```ts
import { Providers } from '@microsoft/mgt';

Providers.globalProvider = myProvider;
```

Todos os componentes serão notificados do novo provedor e começarão a usá-lo.
