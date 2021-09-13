---
title: Crie uma Microsoft Teams SSO com o microsoft Graph Toolkit
description: Começar a criar uma guia Microsoft Teams SSO usando o microsoft Graph Toolkit.
ms.localizationpriority: medium
author: simonagren
ms.openlocfilehash: fe37efb6fc009a862081b6a91a9a34a7c922785b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130609"
---
# <a name="build-a-microsoft-teams-sso-tab-with-the-microsoft-graph-toolkit"></a>Crie uma Microsoft Teams SSO com o microsoft Graph Toolkit

Este tópico descreve como usar o microsoft Graph Toolkit em uma Microsoft Teams solução. Este guia é para um aplicativo de página única com SSO (sign-on único) e exige um back-end. Se você estiver implementando uma guia Teams com login interativo, consulte [Build a Microsoft Teams Tab](./build-a-microsoft-teams-tab.md).

A criação de uma guia SSO envolve as seguintes etapas: 

1. Adicione o microsoft Graph Toolkit.
1. Crie a página pop-up de auth.
1. Criando uma ID de aplicativo/cliente
6. Criar o back-end
7. Inicializar o provedor Teams MSAL2.
8. Adicione os componentes.
9. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o microsoft Graph Toolkit

Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando os pacotes npm. Para usar o Toolkit, você também precisará do [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk).

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
Para usar o Toolkit e Teams SDK por meio dos carregadores, adicione a referência em um script ao seu código:

```HTML
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

A menos que seu aplicativo seja pré-consentido por um administrador, os usuários talvez precisem consentir com permissões. Para habilitar isso, você precisará fornecer uma página que o aplicativo Teams abrirá em um pop-up para seguir o fluxo de autenticação. Você pode fazer com que o caminho para a página seja qualquer coisa, desde que ela seja no mesmo domínio que seu aplicativo (por exemplo, https://yourdomain.com/tabauth) . O único requisito para esta página é chamar o método, mas você `TeamsMsal2Provider.handleAuth()` pode adicionar qualquer conteúdo ou carregar o progresso que quiser.


A seguir está um exemplo de uma página básica que lida com o fluxo de auth no pop-up.

# <a name="unpkg"></a>[unpkg](#tab/unpkg)
```HTML
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
```JavaScript
import { TeamsMsal2Provider } from '@microsoft/mgt-teams-msal2-provider';

TeamsMsal2Provider.handleAuth();
```

---

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Sua guia precisa ser executado como um aplicativo registrado do Azure AD para obter um token de acesso do Azure AD. Registre o aplicativo em seu locatário e Microsoft Teams permissão para obter tokens de acesso em seu nome:

1. Abra um navegador e vá para o centro [de administração Azure Active Directory.](https://aad.portal.azure.com) Entre usando uma **conta pessoal** (Conta da Microsoft) ou Conta de Trabalho **ou Estudante.**

1. No painel esquerdo, selecione **Azure Active Directory**, em seguida, selecione Registros de aplicativo **em** **Gerenciar**.

1. Selecione **Novo registro**. Na página **Registrar um aplicativo**, defina os valores da seguinte forma:

    - Definir **Nome** `Node.js Teams SSO` como (ou um nome de sua escolha).
    - Defina **Tipos de conta com suporte** para **Contas em qualquer diretório organizacional e contas pessoais da Microsoft**.
    - Em **Redirecionar URI**, de definir o primeiro menu suspenso como e definir o valor como a URL da página de autenticação que você criou na etapa `Single Page Application` anterior; por exemplo, `https://myapp.ngrok.io/tabauth` . 

1. Na página visão geral do aplicativo, copie o valor da ID do aplicativo **(cliente)** para posteriormente. Você precisará desse valor ao criar um novo provedor e em seu back-end.

1. Em **Gerenciar**, vá **para Certificados & segredos**. Selecione o botão **Novo segredo do cliente**. Insira um valor em **Descrição** e selecione uma das opções para **Expira** em e selecione **Adicionar**.

1. Copie o valor de segredo do cliente antes de sair desta página. Você precisará disso para seu serviço de back-end.

    >[!IMPORTANT]
    >Este segredo do cliente nunca é mostrado novamente, portanto, certifique-se de copiá-lo agora.

1. Em **Gerenciar**, vá para **permissões de API**. Selecione **Adicionar uma permissão microsoft**  >  **Graph** permissões delegadas , em seguida, adicione as seguintes  >  permissões: , , , `email` , `offline_access` `openid` `profile` `User.Read` . Selecione **Adicionar permissões**.

1. (OPCIONAL) Se você quiser pré-consentimento para quaisquer outros escopos, você pode adicionar mais permissões. Se você usar componentes diferentes ou planejar usar outras APIs Graph Microsoft, talvez seja necessário permissões adicionais. Para obter detalhes sobre permissões necessárias, consulte a [documentação](../overview.md) de cada componente.

    - Para pré-consentimento como administrador, selecione **Conceder consentimento de administrador**, em seguida, selecione **Sim**.

1.  Em **Gerenciar**, vá para **Expor uma API**. Na parte superior da página, ao lado `Application ID URI` de , selecione **Definir**. Isso gera uma API na forma de: `api://{AppID}` . Atualize-o para adicionar seu subdomínio; por exemplo, `api://myapp.ngrok.io/{appID}` .

1. Na mesma página, selecione **Adicionar um escopo**. Preencha os campos da seguinte forma e selecione **Adicionar escopo**:

    - Nome do escopo: `access_as_user`
    - Who podem consentir?: **Administradores e usuários**
    - Nome de exibição de consentimento do administrador: `Teams can access the user’s profile`
    - Descrição do consentimento do administrador: `Allows Teams to call the app’s web APIs as the current user`
    - Nome de exibição de consentimento do usuário: `Teams can access the user profile and make requests on the user's behalf`
    - Descrição do consentimento do usuário: `Enable Teams to call this app’s APIs with the same rights as the user.`
    - Estado: **Habilitado**
    
    Sua URL da API deve ter esta aparência: `api://myapp.ngrok.io/{appID}/access_as_user` . 

1. Em seguida, adicione dois aplicativos cliente. Isso é para os clientes Teams desktop/mobile e o cliente Web. Na seção **Aplicativos cliente autorizados,** selecione **Adicionar um aplicativo cliente**. Preencha a ID do Cliente e selecione o escopo criado. Em seguida, **selecione Adicionar aplicativo**. Faça isso para as seguintes IDs:
    
    - 5e3ce6c0-2b1f-4285-8d4b-75ee78787346
    - 1fec8e78-bce4-4aaf-ab1b-5451cc387264

## <a name="create-the-backend"></a>Criar o back-end

O back-end pode ser qualquer back-end que habilita a troca do token de autenticação Microsoft Teams por um token que pode ser usado para chamar o Microsoft Graph por meio do fluxo [on-behalf-of.](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) 

Para referência, consulte o [Teams SSO Node Sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node).

Veja a seguir uma implementação de referência de um servidor de nó expresso:

```TypeScript
import dotenv from 'dotenv';
import express from 'express';
import path from 'path';
import * as msal from '@azure/msal-node';
import { NextFunction, Request, Response } from 'express';
import jwt, { JwtHeader, SigningKeyCallback } from 'jsonwebtoken';
import jwksClient from 'jwks-rsa';
import jwt_decode from 'jwt-decode';

// Load .env file
dotenv.config();

/**
 * Validates a JWT
 * @param {Request} req - The incoming request
 * @param {Response} res - The outgoing response
 * @returns {Promise<string | null>} - Returns the token if valid, returns null if invalid
 */
function validateJwt(req: Request, res: Response, next: NextFunction): void {
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];
  if (ssoToken) {
    const validationOptions = {
      audience: process.env.CLIENT_ID,
    };
    jwt.verify(ssoToken, getSigningKey, validationOptions, (err, payload) => {
      if (err) {
        return res.sendStatus(403);
      }
      next();
    });
  } else {
    res.sendStatus(401);
  }
}

/**
 * Parses the JWT header and retrieves the appropriate public key
 * @param {JwtHeader} header - The JWT header
 * @param {SigningKeyCallback} callback - Callback function
 */
function getSigningKey(header: JwtHeader, callback: SigningKeyCallback): void {
  const client = jwksClient({
    jwksUri: 'https://login.microsoftonline.com/common/discovery/keys'
  });
  client.getSigningKey(header.kid!, (err, key) => {
    if (err) {
      callback(err, undefined);
    } else {
      callback(null, key.getPublicKey());
    }
  });
}

/**
 * Gets an access token for the user using the on-behalf-of flow
 * @param authHeader - The Authorization header value containing a JWT bearer token
 * @returns {Promise<string | null>} - Returns the access token if successful, null if not
 */
async function getAccessTokenOnBehalfOf(req: Request, res: Response): Promise<void> {
  // The token has already been validated, just grab it
  const authHeader = req.headers.authorization!;
  const ssoToken = authHeader.split(' ')[1];

  // Create an MSAL client
  const msalClient = new msal.ConfidentialClientApplication({
    auth: {
      clientId: req.body.clientid,
      clientSecret: process.env.APP_SECRET
    }
  });

  try {
    const result = await msalClient.acquireTokenOnBehalfOf({
      authority: `https://login.microsoftonline.com/${jwt_decode<any>(ssoToken).tid}`,
      oboAssertion: ssoToken,
      scopes: req.body.scopes,
      skipCache: true
    });
    res.json({ access_token: result?.accessToken });
  } catch (error) {
    if (error.errorCode === 'invalid_grant' || error.errorCode === 'interaction_required') {
      // This is expected if it's the user's first time running the app ( user must consent ) or the admin requires MFA
      res.status(403).json({ error: 'consent_required' }); // This error triggers the consent flow in the client.
    } else {
      // Unknown error
      res.status(500).json({ error: error.message });
    }
  }
}

////////////////////////
// create and run server
////////////////////////

const app = express();
const PORT = process.env.port || process.env.PORT || 8000;

// Support JSON payloads
app.use(express.json());
app.use(express.static(path.join(__dirname, 'client')));

// An example for using POST and with token validation using middleware
app.post('/api/token', validateJwt, async (req, res) => {
  await getAccessTokenOnBehalfOf(req, res);
});

app.listen(PORT, () => {
  console.log(`⚡️[server]: Server is running at http://localhost:${PORT}`);
});
```

## <a name="initialize-the-teams-msal2-provider"></a>Inicializar o provedor Teams MSAL2

Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Teams MSAL2](../providers/teams-msal2.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK Teams para autenticar o usuário.

Para o modo SSO, certifique-se de fornecer e fazer com que ele `sso-url`  /  `ssoUrl` aponte para sua API de back-end.

# <a name="html"></a>[HTML](#tab/HTML)

Adicione o `mgt-teams-msal2-provider` em seu HTML.

```HTML
<mgt-teams-msal2-provider 
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/tabauth"
  scopes="User.Read,Mail.ReadBasic"
  sso-url="http://localhost:8000/api/token"
  http-method="POST"
  ></mgt-teams-msal2-provider>
```

Substitua pela ID do cliente para seu aplicativo, substitua o pelo caminho completo ou relativo para sua página de auth e substitua pelo caminho completo ou relativo para seu serviço `<YOUR_CLIENT_ID>` `auth-popup-url` de `sso-url` back-end.

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

Para inicializar o provedor em seu código JavaScript, importe `TeamsMsal2Provider` e de definir o `globalProvider` .

```TypeScript
import {Providers} from '@microsoft/mgt-element';
import {TeamsMsal2Provider, HttpMethod} from '@microsoft/mgt-teams-msal2-provider';
import * as MicrosoftTeams from "@microsoft/teams-js";

TeamsMsal2Provider.microsoftTeamsLib = MicrosoftTeams;

Providers.globalProvider = new TeamsMsal2Provider({
  clientId: `<YOUR_CLIENT_ID>`,
  authPopupUrl: '/tabauth',
  scopes: ['User.Read','Mail.ReadBasic'],
  ssoUrl: 'http://localhost:8000/api/token',
  httpMethod: HttpMethod.POST
});
```
Substitua pela ID do cliente para seu aplicativo, substitua o pelo caminho completo ou relativo para sua página de auth e substitua pelo caminho completo ou relativo para seu serviço `<YOUR_CLIENT_ID>` `authPopupUrl` de `ssoUrl` back-end.

---

## <a name="add-components"></a>Adicionar os componentes

Agora, você está pronto para adicionar qualquer um dos componentes Graph Toolkit Microsoft. 

Você pode adicionar componentes ao HTML como normalmente faria. Por exemplo, para adicionar o `Person` componente, adicione o código a seguir ao html.

```HTML
<mgt-person person-query="me"></mgt-person>
```

Se você estiver usando React, recomendamos usar os componentes React em vez da `mgt-react` biblioteca. Para saber mais, consulte [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md).

## <a name="test-the-sample"></a>Testar o exemplo
Para a implementação completa, consulte Teams exemplo de [nó SSO](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/teams-sso-node).

Se tudo tiver sido configurado corretamente, você verá o componente `Person` renderizado sem a necessidade de fazer logoff.
>[!IMPORTANT]
>Se você não tiver consentido previamente, talvez seja preciso consentir por meio de um prompt.

## <a name="next-steps"></a>Próximas etapas
- Experimente os componentes do [playground](https://mgt.dev).
- Faça uma pergunta sobre [o Microsoft Q&A](/answers/topics/microsoft-graph-toolkit.html).
- Relate bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
