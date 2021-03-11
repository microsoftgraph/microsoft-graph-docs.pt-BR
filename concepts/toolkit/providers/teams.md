---
title: Provedor do Microsoft Teams
description: Use o provedor do Teams dentro de sua guia do Microsoft Teams para facilitar a autenticação e o acesso do Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 2d4bff6363cc87256f7ec3f9456fbd11f011b48e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719750"
---
# <a name="microsoft-teams-provider"></a>Provedor do Microsoft Teams

Use o provedor do Teams dentro de sua guia do Microsoft Teams para facilitar a autenticação e o acesso do Microsoft Graph a todos os componentes.

Para saber mais sobre provedores de autenticação, consulte [provedores](./providers.md).

>**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsoft Teams com o Provedor do Teams, consulte o guia [Criar uma guia do Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) começando.

## <a name="get-started"></a>Introdução

Antes de usar o provedor do Teams, você precisará se certificar de ter referenciado o [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) do Microsoft Teams em sua página.

# <a name="npm"></a>[npm](#tab/ts)

Instale o kit de ferramentas e o SDK do Microsoft Teams.

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

Em seguida, importe e use o provedor.

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

onde `config` está

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a>atributos mgt-teams-provider
| Atributo | Descrição |
| --- | --- |
| client-id   | ID do cliente de cadeia de caracteres (consulte [Configure your Teams app](#configure-your-teams-app). Obrigatório. |
| auth-popup-url  | Caminho absoluto ou relativo para a página que manipulará a auth no pop-up (consulte [Criar a página pop-up](#create-the-popup-page)). Obrigatório. |
| escopos  | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Opcional. |
| depends-on | Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. |
| authority    | Cadeia de caracteres de autoridade. O padrão é a autoridade comum. Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |

---

### <a name="create-the-popup-page"></a>Criar a página pop-up

Para entrar com suas credenciais do Teams, você precisa fornecer uma URL que o aplicativo do Teams abrirá em um pop-up, que seguirá o fluxo de autenticação. Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método. Essa é a única coisa que essa página precisa fazer. Por exemplo:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a>Configurar URIs de redirecionamento

Depois de publicar a página pop-up em seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade. Essa URL também precisa ser configurada como um URI de redirecionamento válido na configuração do aplicativo no portal do Azure AD.

## <a name="configure-your-teams-app"></a>Configurar seu aplicativo do Teams

Se você está apenas começando com aplicativos do Teams, consulte [Adicionar guias aos aplicativos do Microsoft Teams.](/microsoftteams/platform/concepts/tabs/tabs-overview) Você também pode usar [o App Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.
### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../get-started/add-aad-app-registration.md) no Azure AD. 
>**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth. Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão). Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**. 

## <a name="see-also"></a>Confira também
* [Exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Criar uma guia do Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)