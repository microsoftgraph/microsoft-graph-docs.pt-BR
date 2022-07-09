---
title: Provedor teamsFx
description: Use o provedor TeamsFx dentro de seus aplicativos do Microsoft Teams para fornecer aos componentes do Kit de Ferramentas do Microsoft Graph acesso ao Microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: f5a94ab3fc133ebe38ec552ae152b182000311f7
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698398"
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
// Put this code in a call-to-action callback function to avoid browser blocking automatically showing up pop-ups. 
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

Para obter um exemplo que mostra como inicializar o provedor TeamsFx, consulte o exemplo [exportador de contatos](https://github.com/OfficeDev/TeamsFx-Samples/tree/dev/hello-world-tab-with-backend).


## <a name="see-also"></a>Confira também
* [Introdução ao desenvolvimento do Microsoft Teams e do Kit de Ferramentas do Teams](https://aka.ms/teamsfx-docs)
* [TeamsFx SDK](/microsoftteams/platform/toolkit/teamsfx-sdk)
* [Workshop do Hub de Produtividade](https://github.com/OfficeDev/OneProductivityHub-TeamsFx)
