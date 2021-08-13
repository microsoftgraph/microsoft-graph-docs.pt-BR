---
title: Provedor MSAL 2
description: O provedor MSAL 2 usa o msal-browser para entrar em usuários e adquirir tokens para usar com o microsoft Graph
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: f856c900b0b8aace7a1c2248d2921b39fe0a2c44c6fc9e05c35003c0d0c53d50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54204904"
---
# <a name="msal-2--provider"></a>Provedor MSAL 2

O provedor MSAL 2 usa [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser) para entrar nos usuários e adquirir tokens para usar com o Microsoft Graph.
Para saber mais, confira [provedores](./providers.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor MSAL 2.0 em HTML ou JavaScript.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor MSAL 2 em HTML é a maneira mais simples de criar um novo provedor. Use o `mgt-msal2-provider` componente para definir a **id do** cliente e outras propriedades. Isso criará uma nova instância que será usada para todos os tokens de autenticação `PublicClientApplication` e aquisição.

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
    import {Providers, LoginType} from '@microsoft/mgt-element';
    import {Msal2Provider, PromptType} from '@microsoft/mgt-msal2-provider';

    // initialize the auth provider globally
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes?: string[],
      authority?: string,
      redirectUri?: string,
      loginType?: LoginType, // LoginType.Popup or LoginType.Redirect (redirect is default)
      prompt?: PromptType, // PromptType.CONSENT, PromptType.LOGIN or PromptType.SELECT_ACCOUNT
      sid?: string, // Session ID
      loginHint?: string,
      domainHint?: string,
      options?: Configuration // msal js Configuration object
    });
```

## <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente

Para obter detalhes sobre como registrar um aplicativo e obter uma ID do cliente, consulte [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).

## <a name="difference-between-msal2provider-and-msalprovider"></a>Diferença entre Msal2Provider e MsalProvider
Embora o uso seja muito semelhante, MsalProvider e Msal2Provider são construídos em cima de fluxos OAuth diferentes. O MsalProvider é criado sobre o MSAL.js, que implementa o Flow [.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) Msal2Provider é criado sobre [o msal-browser](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-browser), que implementa o código de autorização [OAuth](/azure/active-directory/develop/v2-oauth2-auth-code-flow) 2.0 Flow com PKCE.
O Código de Autorização Flow é considerado mais seguro do que a concessão implícita Flow aplicativos Web, portanto, recomendamos o uso do MSAL2Provider sobre o MSALProvider. Para obter detalhes sobre problemas de segurança relacionados ao fluxo de concessão implícito, consulte [Desvantagens do fluxo implícito](https://tools.ietf.org/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6).

## <a name="migrating-from-msal-provider-to-msal-2-provider"></a>Migrando do provedor MSAL para o provedor MSAL 2
Para migrar um aplicativo que está usando o provedor MSAL para o Provedor MSAL 2:
1. Vá para o portal do Azure em https://portal.azure.com .
1. No menu, selecione **Azure Active Directory**.
1. No menu Azure Active Directory, selecione **Registros de aplicativos**.
1. Selecione o registro do aplicativo do aplicativo que você está usando no momento. 
1. Vá para **Autenticação** no menu esquerdo.
1. Em **Configurações de plataforma,** clique em **Adicionar uma plataforma** e selecione Aplicativo de página **única.**
1. Remova todas as URIs de redirecionamento que você registrou no momento na **Web** e, em vez disso, **adicione-as** em aplicativo de página única.
1. Em seu código, substitua MSALProvider por MSAL2Provider.

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
