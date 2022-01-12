---
title: Microsoft Teams provedor MSAL2
description: Use o Teams MSAL2 dentro da guia Microsoft Teams para facilitar a autenticação e o acesso Graph Microsoft a todos os componentes. O provedor pode ser usado para SSO (single-sign-on) ou para entrar interativo.
ms.localizationpriority: medium
author: simonagren
ms.openlocfilehash: f46bff605b0980ab71b5ae204e86d90949760117
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862837"
---
# <a name="microsoft-teams-msal2-provider"></a>Microsoft Teams provedor MSAL2

Use o Microsoft Teams MSAL2 dentro da guia Microsoft Teams para facilitar a autenticação e o acesso Graph Microsoft a todos os componentes. O provedor pode ser usado para SSO (login único) ou para entrar interativo.

Para saber mais, confira [provedores](./providers.md).

>**Dica:** Para obter detalhes sobre como criar um aplicativo Microsoft Teams com o provedor Teams MSAL2, consulte [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) and Build a Microsoft Teams tab with [SSO](../get-started/build-a-microsoft-teams-sso-tab.md).


### <a name="difference-between-teams-provider-and-teams-msal2-provider"></a>Diferença entre Teams provedor e Teams MSAL2
Diferentemente do provedor Teams, o provedor Teams MSAL2 dá suporte a SSO (single sign-on) e é criado no [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) para autenticação do lado do cliente. [O msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) implementa o Código de [](/azure/active-directory/develop/v2-oauth2-auth-code-flow) Autorização OAuth 2.0 Flow com PKCE. Como o Código de Autorização Flow é considerado mais seguro do que o Flow de Concessão Implícita para aplicativos Web, recomendamos o uso do provedor Teams MSAL2 no provedor Teams. Para obter detalhes sobre problemas de segurança relacionados ao fluxo de concessão implícito, consulte [Desvantagens do fluxo implícito](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Todos os novos aplicativos devem usar Teams provedor MSAL2 sempre que possível. 

## <a name="get-started"></a>Introdução

O provedor pode ser usado no modo de auth interativo do lado do cliente ou no modo SSO. 

### <a name="client-side-authentication"></a>Autenticação do lado do cliente
Na autenticação do lado do cliente (ou autenticação interativa), o usuário será solicitado a autenticar quando iniciar o aplicativo pela primeira vez. O usuário precisará usar um botão de login para iniciar o fluxo de autenticação. Isso pode ser feito no cliente e não exige um serviço de back-end. 

### <a name="sso-authentication"></a>Autenticação SSO
Para evitar que o usuário se autenture no aplicativo, Microsoft Teams guias também podem [usar o SSO](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) para autenticar automaticamente os usuários. No entanto, esse processo requer um serviço back-end usado para trocar o token Microsoft Teams fornecido por um token de acesso que pode ser usado para acessar o Microsoft Graph.

Teams provedor MSAL2 dá suporte ao modo SSO, que é habilitado quando `ssoUrl`  \  `sso-url` são definidos como um serviço de back-end que é capaz de trocar os tokens. O serviço back-end é necessário para expor uma API (como ) que receberá um token de autenticação do Microsoft Teams e usará o fluxo para trocar o token por um token de acesso que possa acessar o `api/token` `on-behalf-of` Microsoft Graph. Para uma implementação de referência de um serviço de back-end de nó, consulte o [exemplo Microsoft Teams SSO do nó](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).

### <a name="initialize-the-provider"></a>Inicializar o provedor
Antes de usar o Teams MSAL2, certifique-se de fazer referência ao [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) Microsoft Teams em sua página.

Inicializar o provedor Teams MSAL2 no código principal.

# <a name="npm"></a>[npm](#tab/ts)
Ao inicializar o Teams MSAL2 no JavaScript, certifique-se de instalar o kit de ferramentas e o Microsoft Teams SDK.

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider
```

Em seguida, importe e use o provedor.

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider(config);
```

onde `config` está

```ts
export interface TeamsMsal2Config {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
  ssoUrl?: string; // ex: '/api/token',
  autoConsent?: boolean,
  httpMethod: HttpMethod; //ex HttpMethod.POST
}
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="user.read,people.read..." 
  authority=""
  sso-url="/api/token" 
  http-method="POST">
></mgt-teams-msal2-provider>
```

| Atributo | Descrição |
| --- | --- |
| client-id   | ID do cliente de cadeia de caracteres (consulte [Configure your Teams app](#configure-your-teams-app). Obrigatório. |
| auth-popup-url  | Caminho absoluto ou relativo para a página que manipulará a auth no pop-up (consulte [Criar a página pop-up](#create-the-popup-page)). Obrigatório. |
| escopos  | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Opcional. |
| authority    | Cadeia de caracteres de autoridade. O padrão é a autoridade comum. Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário. Por exemplo: `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]`. Opcional. |
| sso-url  | Caminho absoluto ou relativo para a API de back-end que lida com o exchange de tokens OBO. Opcional. |
| http-method  | Tipo de método HTTP a ser usado para chamar a API back-end. `POST` ou `GET`. O padrão é `GET`. Opcional |

---
### <a name="create-the-popup-page"></a>Criar a página pop-up

Para entrar com suas credenciais Teams e manipular o consentimento, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, que seguirá o fluxo de autenticação. Crie uma nova página em seu aplicativo (por exemplo, que manipulará o redirecionamento https://mydomain.com/auth) de auth e chamará o `TeamsMsal2Provider.handleAuth` método. Essa é a única coisa que essa página precisa fazer. Por exemplo:

# <a name="npm"></a>[npm](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;
TeamsMsal2Provider.handleAuth();
```

# <a name="unpkg"></a>[unpkg](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsMsal2Provider.handleAuth();
</script>
```
---

## <a name="configure-your-teams-app"></a>Configurar seu Teams aplicativo

Se você estiver apenas começando a Teams [aplicativos,](/microsoftteams/platform/concepts/tabs/tabs-overview)consulte Adicionar guias a Microsoft Teams aplicativos . Você também pode usar [o App Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver o manifesto do aplicativo.

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente para autenticação [interativa,](../get-started/add-aad-app-registration.md)consulte Create an Azure Active Directory app .


Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente e um segredo para SSO, consulte [Build a Microsoft Teams tab with Single Sign-On](../get-started/build-a-microsoft-teams-sso-tab.md).

## <a name="migrating-from-teams-provider-to-teams-msal2-provider"></a>Migrando do provedor Teams para o Teams MSAL2
Para migrar um aplicativo que está usando o provedor Teams para o provedor Teams MSAL2:
1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu Azure Active Directory, selecione **Registros de aplicativos**.
1. Selecione o registro do aplicativo do aplicativo que você está usando no momento. 
1. No menu esquerdo, vá para **Autenticação**.
1. Em **Configurações de plataforma,** escolha **Adicionar uma plataforma** e selecione Aplicativo de página **única.**
1. Remova todas as URIs de redirecionamento que você registrou no momento na **Web** e, em vez disso, **adicione-as** em aplicativo de página única.
1. Em seu código, substitua o TeamsProvider por Teams Provedor MSAL2.

    Se você estiver inicializando seu provedor no código JS/TS, siga estas etapas:
    
    Substitua a instrução import ```mgt-teams-provider``` por 
    ```ts 
    import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
    ```
    Substituir a inicialização de MsalProvider por
    ```ts
    Providers.globalProvider = new TeamsMsal2Provider(config);
    ```
    Se você estiver inicializando o provedor em HTML, substitua 
    ```html
    <mgt-teams-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-provider>
    ``` 
     com  
    ```html
    <mgt-teams-msal2-provider client-id="<YOUR_CLIENT_ID>" auth-popup-url="/AUTH-PATH" ... ></mgt-teams-msal2-provider>
    ```

## <a name="see-also"></a>Confira também
* [Microsoft Teams de SSO do nó](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [Criar uma guia do Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md)
* [Criar uma Microsoft Teams com SSO](../get-started/build-a-microsoft-teams-sso-tab.md)
