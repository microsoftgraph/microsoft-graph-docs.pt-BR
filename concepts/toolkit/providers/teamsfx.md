---
title: Provedor teamsFx
description: Use o provedor TeamsFx dentro de seus aplicativos do Microsoft Teams para fornecer aos componentes do Kit de Ferramentas do Microsoft Graph acesso ao Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 0789bcff15b523ae8227a2dccf3b0360810fd64e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438238"
---
# <a name="teamsfx-provider"></a>Provedor teamsFx

Use o provedor TeamsFx dentro de seus aplicativos do Microsoft Teams para fornecer aos componentes do Kit de Ferramentas do Microsoft Graph acesso ao Microsoft Graph.

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

Agora você pode adicionar qualquer componente em sua página HTML `render()` ou em seu método ao usar React e ele usará o contexto teamsFx para acessar o Microsoft Graph.

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
* [Introdução ao desenvolvimento do Microsoft Teams e do Kit de Ferramentas do Teams](https://aka.ms/teamsfx-docs)
* [Workshop do Hub de Produtividade](https://github.com/OfficeDev/OneProductivityHub-TeamsFx)
