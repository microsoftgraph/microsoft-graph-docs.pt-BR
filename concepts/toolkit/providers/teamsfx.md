---
title: Provedor TeamsFx
description: Use o provedor TeamsFx dentro de seus aplicativos Microsoft Teams para fornecer aos componentes do Microsoft Graph Toolkit acesso ao Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 62df3d038c7a407da77e92b1d4de04fd1832aacf
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694388"
---
# <a name="teamsfx-provider"></a>Provedor TeamsFx

Use o provedor TeamsFx dentro de seus aplicativos Microsoft Teams para fornecer aos componentes do Microsoft Graph Toolkit acesso ao Microsoft Graph.

Para saber mais sobre provedores de autenticação, consulte [Provedores](./providers.md).

## <a name="get-started"></a>Introdução

Inicialize o provedor dentro do componente.

```ts
// Import the providers and credential at the top of the page
import {Providers} from '@microsoft/mgt-element';
import {TeamsFxProvider} from '@microsoft/mgt-teamsfx-provider';
import {TeamsUserCredential} from "@microsoft/teamsfx";

const scope = ["User.Read"];
const teamsfx = new TeamsFx();
const provider = new TeamsFxProvider(teamsfx, scope);
Providers.globalProvider = provider;
```

Use o `teamsfx.login(scopes)` método para obter o token de acesso necessário.

```ts
// Automatically when loading the component or in a call-to-action
await teamsfx.login(this.scope);
Providers.globalProvider.setState(ProviderState.SignedIn);
```

Agora você pode adicionar qualquer componente em sua página HTML `render()` ou em seu método ao usar React e ele usará o contexto do TeamsFx para acessar o Microsoft Graph.

```html
<!-- Using HTML -->
<mgt-person query="me" view="threeLines"></mgt-person>
```

```ts
// Using React
public render(): void {
  return (
      <div>
        <Person personQuery="me" view={PersonViewType.threelines}></Person>
      </div>
  );
}
```

Para obter um exemplo que mostra como inicializar o provedor TeamsFx, consulte o exemplo [exportador de contatos](https://github.com/OfficeDev/TeamsFx-Samples/tree/ga/graph-toolkit-contact-exporter).

## <a name="see-also"></a>Confira também
* [Introdução com Microsoft Teams e Teams Toolkit desenvolvimento](https://aka.ms/teamsfx-docs)
