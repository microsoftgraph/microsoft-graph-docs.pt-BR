---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 57d53d19507e3ad6d53810538eff62a0e20740bd
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275693"
---
# <a name="microsoft-teams-provider"></a>Provedor do Microsoft Teams

Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.

Para saber mais, veja [Providers](../providers.md).

## <a name="get-started"></a>Introdução

Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) na sua página.

### <a name="via-script-tag"></a>via marca de script
O exemplo a seguir usa o provedor em HTML (via CDN).

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

| Atributo | Descrição |
| --- | --- | --- |
| Client-ID   | String Client ID (consulte Configure Your Teams app). Obrigatório. |
| auth-Popup-URL  | Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte criar a página pop-up). Obrigatório. |
| escopos  | Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar. Opcional. |
| depende de | Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. |

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

Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview). Você também pode usar o [app Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.

Após instalar seu aplicativo com uma guia e você estiver pronto para usar os componentes, você precisará certificar-se de que seu aplicativo tem as permissões corretas para acessar o Microsoft Graph. Para configurar seu aplicativo com as permissões necessárias:

1. [Recuperar seu nome de domínio](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [Criar um novo registro de aplicativo](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [Conceder sua permissão de aplicativo](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

É importante adicionar a permissão certa na **página Adicionar acesso à API**. Você precisará de um administrador para adicionar e aprovar as permissões, dependendo de qual componente você precisa.

>**Dica:** Se você não tiver certeza sobre as permissões a serem adicionadas, consulte a documentação de cada componente.

### <a name="enable-implicit-grant-flow"></a>Habilitar fluxo de concessão implícito

Certifique-se de habilitar o fluxo de concessão implícito; Esse é um requisito para aplicativos Web que solicitam tokens do lado do cliente. No portal do Azure, ao gerenciar o registro do aplicativo, edite o manifesto `oauth2AllowImplicitFlow` e `true`altere para.

### <a name="create-the-popup-page"></a>Criar a página pop-up

Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação. Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método. Essa é a única coisa que esta página precisa fazer. Por exemplo:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

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
