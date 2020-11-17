---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b102d216b9a9b4181fa070c6c95f543098fa0ba0
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086603"
---
# <a name="microsoft-teams-provider"></a>Provedor do Microsoft Teams

Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.

Para saber mais sobre provedores de autenticação, consulte [Providers](../providers.md).

>**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsot Teams com o provedor Teams, consulte o guia [criar uma guia de introdução ao Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) .

## <a name="get-started"></a>Introdução

Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) na sua página.

### <a name="via-script-tag"></a>via marca de script
O exemplo a seguir usa o provedor em HTML (via CDN).

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| Atributo | Descrição |
| --- | --- |
| Client-ID   | ID do cliente de cadeia de caracteres (consulte [Configure Your Teams app](#configure-your-teams-app). Obrigatório. |
| auth-Popup-URL  | Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte [criar a página pop-up](#create-the-popup-page)). Obrigatório. |
| escopos  | Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar. Opcional. |
| depende de | Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. |
| autoridades    | Cadeia de caracteres de autoridade. O padrão é a autoridade comum. Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |


### <a name="via-npm"></a>via NPM
O exemplo a seguir usa o provedor em módulos JS (via NPM).

Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

Em seguida, importe e use o provedor.

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

onde `config` é

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

Como alternativa, você pode precisar definir a referência à biblioteca do Microsoft Teams. Veja um exemplo:

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

Para ver um exemplo completo, confira o [exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).

## <a name="configure-your-teams-app"></a>Configurar seu aplicativo do teams

Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview). Você também pode usar o [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.

Após instalar seu aplicativo com uma guia e você estiver pronto para usar os componentes, você precisará certificar-se de que seu aplicativo tem as permissões corretas para acessar o Microsoft Graph. Para configurar seu aplicativo com as permissões necessárias:

1. [Recuperar seu nome de domínio](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [Criar um novo registro de aplicativo](../get-started/add-aad-app-registration.md)
3. [Conceder sua permissão de aplicativo](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

É importante adicionar a permissão certa na **página Adicionar acesso à API**. Você precisará de um administrador para adicionar e aprovar as permissões, dependendo de qual componente você precisa.

>**Dica:** Se você não tiver certeza sobre as permissões a serem adicionadas, consulte a documentação de cada componente.

### <a name="enable-implicit-grant-flow"></a>Habilitar fluxo de concessão implícito

Certifique-se de habilitar o fluxo de concessão implícito; Esse é um requisito para aplicativos Web que solicitam tokens do lado do cliente. No portal do Azure, ao gerenciar o registro do aplicativo, edite o manifesto e altere `oauth2AllowImplicitFlow` para `true` .

### <a name="create-the-popup-page"></a>Criar a página pop-up

Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação. Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método. Essa é a única coisa que esta página precisa fazer. Por exemplo:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

ou por um módulo mencionado na página pop-up de autenticação:

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a>Configurar URIs de redirecionamento

Após publicar esta página no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade. Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.
