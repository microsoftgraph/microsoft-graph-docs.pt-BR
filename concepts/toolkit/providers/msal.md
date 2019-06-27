---
title: Provedor MSAL
description: O provedor MSAL usa MSAL. js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242937"
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
                   authority=""></mgt-msal-provider>
```

>**Observação:** `login-type` e `authority` são opcionais.

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

>**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para tokens de **acesso** e tokens de **ID**.
