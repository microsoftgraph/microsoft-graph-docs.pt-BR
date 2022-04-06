---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar em usuários e adquirir tokens para usar com o microsoft Graph.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 08c12c4ba7b105573e7a19a705a804c5c9f92114
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587036"
---
# <a name="msal-provider"></a>Provedor MSAL

O Provedor MSAL usa [msal.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, confira [provedores](./providers.md).

## <a name="difference-between-msal2-provider-and-msal-provider"></a>Diferença entre Provedor MSAL2 e Provedor MSAL
Embora o uso seja semelhante, o Provedor MSAL e o Provedor MSAL2 são construídos em fluxos OAuth diferentes. O Provedor MSAL é criado msal.js, que implementa o [Flow.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) O Provedor MSAL2 é criado no [msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), que implementa o Código de Autorização [OAuth](/azure/active-directory/develop/v2-oauth2-auth-code-flow) 2.0 Flow com PKCE.
Como o Código de Autorização Flow é considerado mais seguro do que a concessão implícita Flow aplicativos Web, recomendamos usar o Provedor MSAL2 em relação ao Provedor MSAL. Para obter detalhes sobre problemas de segurança relacionados ao fluxo de concessão implícito, consulte [Desvantagens do fluxo implícito](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Todos os novos aplicativos devem usar o Provedor MSAL2 sempre que possível. Para obter informações de migração, consulte [Provedor MSAL2](./msal2.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor MSAL em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal-provider` componente para definir a **id do** cliente e outras propriedades. Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""
                   domainHint="mydomain.com"
                   prompt="consent"></mgt-msal-provider>
```

| Atributo    | Descrição                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente). Obrigatório.                                                                                                                                                                                                           |
| tipo de logon   | Enumeração entre `redirect` e `popup` - o valor padrão é `redirect`. Opcional.                                                                                                                                                                                   |
| escopos       | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Opcional.                                                                                                                                                                                     |
| authority    | Cadeia de caracteres de autoridade - padrão é a autoridade comum. Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário. Por exemplo: `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]`. Opcional. |
| redirect-uri | Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado. Opcional.                                                                                                                                                                                            |
| depends-on   | Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta. Opcional. 
| domain-hint  | Cadeia de caracteres de consulta do local do domínio para encaminhamento da experiência de login. Opcional.              
| prompt | Seleção para o tipo de interação do usuário necessário para fazer logon. As opções válidas incluem: <ul><li>`login` força o usuário a inserir credenciais à solicitação </li><li>`none` para nenhum prompt interativo</li> <li>`select_account` para enviar o usuário para um selador de conta</li><li>`consent` para enviar o usuário para uma caixa de diálogo de consentimento OAuth</li></ul> Para obter mais informações de prompt, consulte [o comportamento do prompt no MSAL.js](/azure/active-directory/develop/msal-js-prompt-behavior) artigo. Opcional.                                                                                                                                                                            |


### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor em JavaScript.

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

Você pode configurar o `MsalProvider` parâmetro construtor de duas maneiras, conforme descrito nas seções a seguir.

#### <a name="provide-a-clientid-to-create-a-new-useragentapplication"></a>Fornecer um `clientId` para criar um novo `UserAgentApplication`

Essa opção faz sentido quando Graph Toolkit é responsável por toda a autenticação em seu aplicativo.

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
  domainHint?: string;
  prompt?: string; // "login", "none", "select_account", "consent"
}
```

#### <a name="pass-an-existing-useragentapplication-in-the-useragentapplication-property"></a>Passe um existente `UserAgentApplication` na `userAgentApplication` propriedade.

Use isso quando seu aplicativo usa a funcionalidade MSAL `MsalProvider` além do que é exposto pelo microsoft Graph Toolkit recursos. Isso é particularmente apropriado se uma estrutura instancie `UserAgentApplication` e exponha automaticamente um para você; por exemplo, ao usar [msal-angular](/azure/active-directory/develop/tutorial-v2-angular).

Certifique-se de entender as oportunidades de colisões ao usar essa opção. Por sua própria natureza, `MsalProvider` há o risco de que o estado de uma sessão possa mudar, por exemplo, fazendo com que o usuário entre ou consenta com escopos adicionais. Certifique-se de que seu aplicativo e outras estruturas respondam normalmente a essas alterações no estado ou considere usar um [provedor personalizado](./custom.md) em vez disso.

```ts
interface MsalConfig {
  userAgentApplication: UserAgentApplication;
  scopes?: string[];
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string;
}
```

Para saber mais sobre MSAL.js opções adicionais que você pode usar ao inicializar a biblioteca MSAL, consulte a [documentação do MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).
