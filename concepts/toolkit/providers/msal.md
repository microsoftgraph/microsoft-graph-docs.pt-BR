---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: d3b3d82ae3c60080beaaff7f39a1324022d3ab2a
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659161"
---
# <a name="msal-provider"></a>Provedor MSAL

O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, veja [Providers](./providers.md).

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

Você pode configurar o `MsalProvider` parâmetro constructor de duas maneiras, conforme descrito nas seções a seguir.

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>Fornecer um `clientId` para criar um novo `UserAgentApplication`

Essa opção faz sentido quando o kit de ferramentas do Graph é responsável por toda a autenticação em seu aplicativo.

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

Use isso quando o aplicativo usar a funcionalidade do MSAL além do que está exposto pelo `MsalProvider` e outros recursos do Microsoft Graph Toolkit. Isso é especialmente apropriado se uma estrutura instancia automaticamente e expõe uma `UserAgentApplication` por você; por exemplo, ao usar [MSAL-angular](https://docs.microsoft.com/azure/active-directory/develop/tutorial-v2-angular).

Certifique-se de entender as oportunidades de colisões ao usar essa opção. Por sua própria natureza, há um risco de `MsalProvider` alterar o estado de uma sessão, por exemplo, fazendo com que o usuário entre ou concorde com escopos adicionais. Certifique-se de que seu aplicativo e outras estruturas respondam adequadamente a essas alterações no estado ou considere o uso de um [provedor personalizado](/graph/toolkit/providers/custom) .

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Para saber mais sobre MSAL.js e para opções adicionais que você pode usar ao inicializar a biblioteca do MSAL, consulte a [documentação do MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte [criar um aplicativo do Azure Active Directory](../get-started/add-aad-app-registration.md).
