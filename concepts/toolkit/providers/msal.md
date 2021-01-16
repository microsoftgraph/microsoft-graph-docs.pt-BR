---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 738e8ebcd24b3e7e528bdf0a1676dd54103ee2ea
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883022"
---
# <a name="msal-provider"></a>Provedor MSAL

O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, consulte [provedores.](./providers.md)

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor MSAL em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades. Isso criará uma nova `UserAgentApplication` instância que será usada para toda a autenticação e aquisição de tokens.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| Atributo    | Descrição                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente). Obrigatório.                                                                                                                                                                                                           |
| tipo de logon   | Enumeração entre `redirect` e - o valor padrão é `popup` `redirect` . Opcional.                                                                                                                                                                                   |
| escopos       | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Opcional.                                                                                                                                                                                     |
| autoridade    | Cadeia de caracteres de autoridade – o padrão é a autoridade comum. Para aplicativos de locatário único, use a ID do locatário ou o nome do locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |
| redirect-uri | Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado. Opcional.                                                                                                                                                                                            |
| depende   | Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional.                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor em JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

Você pode configurar o `MsalProvider` parâmetro do construtor de duas maneiras, conforme descrito nas seções a seguir.

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>Fornecer um `clientId` para criar um novo `UserAgentApplication`

Essa opção faz sentido quando o Graph Toolkit é responsável por toda a autenticação em seu aplicativo.

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

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>Passe um existente `UserAgentApplication` na `userAgentApplication` propriedade.

Use isso quando seu aplicativo usa a funcionalidade MSAL além do que é exposto pelos recursos e outros recursos do `MsalProvider` Microsoft Graph Toolkit. Isso é particularmente apropriado se uma estrutura instanciá-la automaticamente e expor uma para você; por exemplo, ao usar `UserAgentApplication` [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).

Certifique-se de entender as oportunidades de colisões ao usar essa opção. Por sua própria natureza, há um risco de que o estado de uma sessão possa ser diferente, por exemplo, fazendo o usuário entrar ou consentir com `MsalProvider` escopos adicionais. Certifique-se de que seu aplicativo e outras estruturas respondam normalmente a essas alterações de estado ou considere usar um [provedor personalizado.](./custom.md)

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Para saber mais sobre MSAL.js e para opções adicionais que você pode usar ao inicializar a biblioteca MSAL, consulte a documentação [da MSAL.](/azure/active-directory/develop/msal-js-initializing-client-applications)

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte [Criar um aplicativo do Azure Active Directory.](../get-started/add-aad-app-registration.md)