---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c3c921cfa473e2001d2a150096741d2bddf39f10
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288158"
---
# <a name="msal-provider"></a>Provedor MSAL

O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, veja [Providers](../providers.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor MSAL em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar na página HTML

Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades. Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| Atributo    | Descrição                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Client-ID    | String Client ID (consulte Creating a app/Client ID). Obrigatório.                                                                                                                                                                                                           |
| tipo de logon   | A enumeração entre `redirect` e o `popup` valor padrão é `redirect` . Opcional.                                                                                                                                                                                   |
| escopos       | Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar. Opcional.                                                                                                                                                                                     |
| autoridades    | A cadeia de caracteres de autoridade-padrão é a autoridade comum. Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |
| Redirect-URI | Redirecionar cadeia de caracteres URI-por padrão, o URI de janela atual é usado. Opcional.                                                                                                                                                                                            |
| depende de   | Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional.                                                                                                                                                                                      |

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
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication` ).

Para saber mais sobre MSAL.js e para opções adicionais que você pode usar ao inicializar a biblioteca do MSAL, consulte a [documentação do MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte o [início rápido registrar um aplicativo](/azure/active-directory/develop/quickstart-register-app).

>**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**. Para usar a autoridade comum, defina **Account em qualquer diretório organizacional**. Para usar um locatário específico, defina o `authority` durante a inicialização.