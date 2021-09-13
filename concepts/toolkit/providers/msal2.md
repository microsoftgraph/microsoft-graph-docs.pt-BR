---
title: Provedor MSAL2
description: O provedor MSAL 2 usa o msal-browser para entrar em usuários e adquirir tokens para usar com o microsoft Graph
ms.localizationpriority: medium
author: amrutha95
ms.openlocfilehash: 80178f379d0f6d9101cec794bc1d0d36ccb640d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143479"
---
# <a name="msal2-provider"></a>Provedor MSAL2

O Provedor MSAL2 usa [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.

Para saber mais, confira [provedores](./providers.md).

## <a name="difference-between-msal2-provider-and-msal-provider"></a>Diferença entre Provedor MSAL2 e Provedor MSAL
Embora o uso seja semelhante, o Provedor MSAL e o Provedor MSAL2 são construídos em fluxos OAuth diferentes. O Provedor MSAL é criado msal.js, que implementa o Flow [.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) O Provedor MSAL2 é criado com [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), que implementa o código de autorização [OAuth](/azure/active-directory/develop/v2-oauth2-auth-code-flow) 2.0 Flow com PKCE.
Como o Código de Autorização Flow é considerado mais seguro do que o Flow de Concessão Implícita para aplicativos Web, recomendamos usar Msal2Provider sobre MsalProvider. Para obter detalhes sobre problemas de segurança relacionados ao fluxo de concessão implícito, consulte [Desvantagens do fluxo implícito](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

Todos os novos aplicativos devem usar o Provedor MSAL2 sempre que possível. 

## <a name="get-started"></a>Introdução

Você pode inicializar o Provedor MSAL2 em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor MSAL2 em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal2-provider` componente para definir a **id do** cliente e outras propriedades. Isso criará uma nova instância que será usada para todos os tokens de autenticação `PublicClientApplication` e aquisição.

```html
    <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"
                        login-type="redirect/popup" 
                        scopes="user.read,people.read" 
                        redirect-uri="https://my.redirect/uri" 
                        authority=""> 
    </mgt-msal2-provider> 
```

| Atributo    | Descrição                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client-id    | ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente). Obrigatório.                                                                                                                                                                                                           |
| tipo de logon   | Enumeração entre `redirect` e - o valor padrão é `popup` `redirect` . Opcional.                                                                                                                                                                                   |
| escopos       | Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar. Opcional.                                                                                                                                                                                     |
| authority    | Cadeia de caracteres de autoridade - padrão é a autoridade comum. Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário. Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` . Opcional. |
| redirect-uri | Cadeia de caracteres de URI de redirecionamento - por padrão, o URI da janela atual é usado. Opcional.                                                                                                                                                                                            |
| prompt       | Tipo de prompt a ser usado para logon, entre ```SELECT_ACCOUNT``` e ```CONSENT``` ```LOGIN``` . O padrão é ```SELECT_ACCOUNT```. Opcional.

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor em JavaScript.

```ts
    import {Providers} from '@microsoft/mgt-element';
    import {Msal2Provider, Msal2Config, Msal2PublicClientApplicationConfig} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider(config: Msal2Config | Msal2PublicClientApplicationConfig);
```

Você pode configurar o `Msal2Provider` parâmetro construtor de duas maneiras, conforme descrito nas seções a seguir.

#### <a name="provide-a-clientid-to-create-a-new-publicclientapplication"></a>Fornecer um `clientId` para criar um novo `PublicClientApplication`

Essa opção faz sentido quando o microsoft Graph Toolkit é responsável por toda a autenticação em seu aplicativo.

```ts
interface Msal2Config {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

#### <a name="pass-an-existing-publicclientapplication-in-the-publicclientapplication-property"></a>Passe um existente `PublicClientApplication` na `publicClientApplication` propriedade.

Use isso quando seu aplicativo usa a funcionalidade MSAL além do que é exposto pelos recursos `Msal2Provider` do Microsoft Graph Toolkit. Isso é particularmente apropriado se uma estrutura instancie e exponha automaticamente um para você; por exemplo, ao `PublicClientApplication` usar [msal-angular](/azure/active-directory/develop/tutorial-v2-angular). Para obter mais orientações, consulte `angular-app` o exemplo no microsoft Graph Toolkit [repo](https://github.com/microsoftgraph/microsoft-graph-toolkit).

Certifique-se de entender as oportunidades de colisões ao usar essa opção. Por sua própria natureza, há o risco de que o estado de uma sessão possa ser alterado; por exemplo, fazendo com que o usuário entre ou consenta com `Msal2Provider` escopos adicionais. Certifique-se de que seu aplicativo e outras estruturas respondam normalmente a essas alterações no estado ou considere usar um [provedor personalizado](./custom.md) em vez disso.

```ts
interface Msal2PublicClientApplicationConfig {
  publicClientApplication: PublicClientApplication;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  prompt?: PromptType; // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
  sid?: string; // Session ID
  loginHint?: string;
  domainHint?: string;
  options?: Configuration // msal-browser Configuration object
}
```

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).

## <a name="migrating-from-msal-provider-to-msal2-provider"></a>Migrando do provedor MSAL para o provedor MSAL2
Para migrar um aplicativo que está usando o provedor MSAL para o Provedor MSAL2:
1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu Azure Active Directory, selecione **Registros de aplicativos**.
1. Selecione o registro do aplicativo do aplicativo que você está usando no momento. 
1. Vá para **Autenticação** no menu esquerdo.
1. Em **Configurações de plataforma,** clique em **Adicionar uma plataforma** e selecione Aplicativo de página **única.**
1. Remova todas as URIs de redirecionamento que você registrou no momento na **Web** e, em vez disso, **adicione-as** em aplicativo de página única.
1. Em seu código, substitua `MSALProvider` por `MSAL2Provider` .

    Se você estiver inicializando seu provedor no código JS/TS, siga estas etapas:
    
    Substitua a instrução import ```mgt-msal-provider``` por 
    ```ts 
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';
    ```

    Substituir a inicialização de MsalProvider por
    ```ts
    Providers.globalProvider = new Msal2Provider({ 
      clientId: 'REPLACE_WITH_CLIENTID'
      ...
    })
    ```
    Se você estiver inicializando o provedor em HTML, substitua 
    ```html
    <mgt-msal-provider client-id="" ... ></mgt-msal-provider>
    ``` 
    com 
    ```html
    <mgt-msal2-provider  client-id="" ... ></mgt-msal2-provider>
     ```
    Para obter detalhes, [consulte Inicializar em sua página HTML](#initialize-in-your-html-page).
