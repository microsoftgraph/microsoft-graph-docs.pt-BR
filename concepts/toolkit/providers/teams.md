---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 463fa4afdfd4e0dd3e3cb09ad155f0cae08fb347
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664034"
---
# <a name="microsoft-teams-provider"></a>Provedor do Microsoft Teams

Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.

Para saber mais sobre provedores de autenticação, consulte [Providers](./providers.md).

>**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsoft Teams com o provedor Teams, consulte o guia criar um guia de introdução ao [Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) .

## <a name="get-started"></a>Introdução

Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) na sua página.

# <a name="npm"></a>[npm](#tab/ts)

Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

Em seguida, importe e use o provedor.

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

onde `config` é

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

### <a name="mgt-teams-provider-attributes"></a>provedores de gerenciamento de equipes
| Atributo | Descrição |
| --- | --- |
| Client-ID   | ID do cliente de cadeia de caracteres (consulte [Configure Your Teams app](#configure-your-teams-app). Obrigatório. |
| auth-Popup-URL  | Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte [criar a página pop-up](#create-the-popup-page)). Obrigatório. |
| escopos  | Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar. Opcional. |
| depende de | Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. |
| autoridades    | Cadeia de caracteres de autoridade. O padrão é a autoridade comum. Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |

---

### <a name="create-the-popup-page"></a>Criar a página pop-up

Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação. Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método. Essa é a única coisa que esta página precisa fazer. Por exemplo:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
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

Após publicar a página pop-up no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade. Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.

## <a name="configure-your-teams-app"></a>Configurar seu aplicativo do teams

Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview). Você também pode usar o [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.
### <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente
Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../get-started/add-aad-app-registration.md) no Azure AD. 
>**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**. 

## <a name="see-also"></a>Também consulte
* [Exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Criar uma guia do Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)