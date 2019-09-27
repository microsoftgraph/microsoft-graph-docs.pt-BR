---
title: Provedor MSAL
description: O provedor MSAL usa MSAL. js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0e8b0b52780e3e4449a0aef0b440ad39f105c85b
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275714"
---
# <a name="msal-provider"></a>Provedor MSAL

O provedor MSAL usa [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, veja [Providers](../providers.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor MSAL em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar na página HTML

Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades. Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| Atributo | Descrição |
| --- | --- | --- |
| Client-ID   | String Client ID (consulte Creating a app/Client ID). Obrigatório.|
| tipo de logon  | A enumeração `redirect` entre `popup` e o valor padrão `redirect`é. Opcional. |
| escopos  | Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar. Opcional.|
| autoridades  | A cadeia de caracteres de autoridade-padrão é a autoridade comum. Opcional.|
| depende de | Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. |

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor no JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

onde MsalConfig é:

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication`).

Para saber mais, confira a [documentação do MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).

## <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte o [início rápido registrar um aplicativo](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).

>**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.
