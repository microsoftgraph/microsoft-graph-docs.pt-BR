---
title: Crie uma Microsoft Teams com o microsoft Graph Toolkit
description: Começar a criar uma guia Microsoft Teams usando o microsoft Graph Toolkit.
ms.localizationpriority: medium
author: simonagren
ms.openlocfilehash: ac3309a0954cd7426b4399aca2043ff811f00c6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129555"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Crie uma Microsoft Teams com o microsoft Graph Toolkit

Este tópico aborda como começar a usar o microsoft Graph Toolkit em uma solução Microsoft Teams. Este guia é para um aplicativo de página única sem SSO (SSO) e não exige um back-end. Se você estiver implementando o SSO com um back-end personalizado, consulte [Build a Microsoft Teams tab (SSO)](./build-a-microsoft-teams-sso-tab.md).

A criação de uma guia envolve as seguintes etapas:

1. Adicione o microsoft Graph Toolkit.
1. Crie a página pop-up de auth.
1. Criando uma ID de aplicativo/cliente
1. Inicializar o provedor Teams MSAL2.
1. Adicione os componentes.
1. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o microsoft Graph Toolkit

Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando os pacotes npm. Para usar o Toolkit, você também precisará do [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk).

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
Para usar o Toolkit e Teams SDK por meio dos carregadores, adicione a referência em um script ao seu código:

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

# <a name="npm"></a>[npm](#tab/npm)
Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione os pacotes npm para o Toolkit e o SDK Microsoft Teams ao seu projeto:

```cmd
npm install @microsoft/teams-js @microsoft/mgt-element @microsoft/mgt-teams-msal2-provider @microsoft/mgt-components
```

---

## <a name="create-the-auth-popup-page"></a>Criar a página pop-up de auth

Para permitir que os usuários entre, você precisará de uma página em seu aplicativo que Teams abrirá em um pop-up para seguir o fluxo de autenticação. O caminho para a página pode ser qualquer coisa desde que ele seja no mesmo domínio que seu aplicativo (por exemplo, https://yourdomain.com/tabauth) . O único requisito para esta página é chamar o método, mas você `TeamsMsal2Provider.handleAuth()` pode adicionar qualquer conteúdo ou carregar o progresso que quiser.

A seguir, um exemplo de página básica que lida com o fluxo de auth no pop-up.

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsMsal2Provider.handleAuth();
    </script>
  </body>
</html>
```
# <a name="npm"></a>[npm](#tab/npm)
```js
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar um aplicativo Azure Active Directory cliente. Siga as etapas no [artigo Criar um Azure Active Directory app.](./add-aad-app-registration.md)

Certifique-se de definir o registro no aplicativo para apontar para `redirect URI` a página de auth que você criou na etapa anterior. Por exemplo, https://localhost:3000/tabauth.

> **Observação:** Certifique-se de definir `redirect URI` o como `Single Page Application (SPA)` um . Teams O Provedor MSAL2 faz uso do Provedor MSAL2 nos bastidores.

## <a name="initialize-the-teams-msal2-provider"></a>Inicializar o provedor Teams MSAL2

Os provedores do Kit de ferramentas do Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Teams provedor MSAL2](../providers/teams-msal2.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK Teams para autenticar o usuário.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

# <a name="html"></a>[html](#tab/html)


Adicione o `mgt-teams-msal2-provider` componente à sua página HTML conforme mostrado.

```html
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  ></mgt-teams-msal2-provider>
```

Substitua pela ID do cliente para seu aplicativo e substitua o pelo caminho completo ou `<YOUR_CLIENT_ID>` relativo para sua página de `auth-popup-url` auth. 

# <a name="js"></a>[js](#tab/js)


Para inicializar o provedor em seu código JavaScript, adicione o seguinte código ao seu aplicativo:

```ts
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
});
```
Substitua pela ID do cliente para seu aplicativo e substitua o pelo caminho completo ou `<YOUR_CLIENT_ID>` relativo para sua página de `authPopupUrl` auth.

---
## <a name="add-components"></a>Adicionar os componentes

Agora, você está pronto para adicionar qualquer um dos componentes Graph Toolkit Microsoft. O primeiro componente que você provavelmente precisará adicionar é o componente Logon.

```HTML
<mgt-login></mgt-login>
```

O componente Logon renderiza um botão "Entrar" que orienta o usuário pelo processo de logon e se integra a qualquer um dos provedores para lidar com a autenticação. Depois que o usuário entrar, todos os outros componentes do kit de ferramentas poderão chamar a Microsoft Graph automaticamente. Os provedores também expõem um cliente microsoft Graph autenticado para fazer chamadas de API ou obter tokens de acesso. Para obter detalhes, consulte [Using the providers](../providers/providers.md).

Se você estiver usando React, recomendamos usar os componentes React em vez da `mgt-react` biblioteca. Para saber mais, consulte [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)

## <a name="next-steps"></a>Próximas etapas
- Experimente os componentes do [playground](https://mgt.dev).
- Faça uma pergunta sobre [o Microsoft Q&A](/answers/topics/microsoft-graph-toolkit.html).
- Relate bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
