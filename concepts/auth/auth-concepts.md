---
title: Princípios Básicos de Autenticação e Autorização para o Microsoft Graph
description: Para chamar o Microsoft Graph, o aplicativo deve adquirir um token de acesso da Microsoft Identity Plataform.
author: matt-steele
localization_priority: Priority
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 8e38f8914caf1ccfb024f4ab96de03cf9a6140c5
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474369"
---
# <a name="authentication-and-authorization-basics-for-microsoft-graph"></a>Princípios Básicos de Autenticação e Autorização para o Microsoft Graph

Para chamar o Microsoft Graph, seu aplicativo deve adquirir um token de acesso da plataforma de identidade da Microsoft. O token de acesso contém informações sobre o aplicativo e as permissões que ele tem para os recursos e APIs disponíveis no Microsoft Graph. Para obter um token de acesso, o aplicativo deve ser registrado na plataforma de identidade da Microsoft e ter a autorização de um usuário ou administrador para acessar os recursos necessários do Microsoft Graph.

Este tópico fornece uma visão geral dos tokens de acesso, da Microsoft Identidade Platform e de como seu aplicativo pode obter tokens de acesso. Se você já estiver familiarizado com a integração de um aplicativo com o Microsoft Identity Platform para obter tokens, confira a seção [Próximas Etapas](#next-steps) para obter informações e exemplos específicos do Microsoft Graph.

## <a name="access-tokens"></a>Tokens de acesso

Os tokens de acesso emitidos pela plataforma de identidade da Microsoft contêm informações (declarações) que as APIs da Web protegidas pela plataforma de identidade da Microsoft, como o Microsoft Graph, usam para validar o chamador e para garantir que o chamador tenha as permissões adequadas para executar a operação solicitada. Ao chamar o Microsoft Graph, trate os tokens de acesso como opacos. Sempre transmita os tokens de acesso através de um canal seguro, tal como o protocolo TLS (HTTPS).

Este é um exemplo de token de acesso da plataforma de identidade da Microsoft:

```jwt
EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

Para chamar o Microsoft Graph, anexe o token de acesso como um token de portador ao cabeçalho de autorização em uma solicitação HTTP. Por exemplo, a seguinte chamada que retorna as informações de perfil do usuário conectado (o token de acesso foi abreviado para facilitar a leitura):

```http
GET https://graph.microsoft.com/v1.0/me/ HTTP/1.1
Host: graph.microsoft.com
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

## <a name="register-your-app-with-the-microsoft-identity-platform"></a>Registre um aplicativo na Microsoft Identity Platform

Antes que seu aplicativo possa receber um token da Microsoft Identity Platform, ele deve ser registrado no [portal do Azure](https://portal.azure.com/). O registro integra o aplicativo com a Microsoft Identity Platform e estabelece as informações que ele usa para acessar os tokens, incluindo:

- **ID do aplicativo**: um identificador exclusivo atribuído pela Microsoft Identity Platform.
- **Redirecionamento de URL/URI**: um ou mais pontos de extremidade no qual seu aplicativo receberá respostas da Microsoft Identity Platform. (Para aplicativos móveis e nativos, será um URI atribuído pela Microsoft Identity Platform.)
- **Segredo do Aplicativo**: uma senha ou um par de chaves públicas/particulares que seu aplicativo usa para se autenticar com a Microsoft Identity Platform. (Não é necessário para aplicativos nativos ou móveis.)

As propriedades definidas durante o registro são usadas na solicitação. Por exemplo, na solicitação de token a seguir: *client_id* é a *ID do Aplicativo*, *redirect_uri* é um *URIs de Redirecionamento* de seu aplicativo registrado, e *client_secret* é o *Segredo do Aplicativo*.

```http
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

O Microsoft Graph expõe permissões granulares que controlam o acesso de aplicativos a recursos, como usuários, grupos e email. Como desenvolvedor, você decide quais permissões solicitar ao Microsoft Graph. Quando um usuário faz logon no aplicativo, ele ou, em alguns casos, um administrador, tem a chance de consentir essas permissões. Se o usuário consentir, o aplicativo receberá acesso aos recursos e APIs solicitados. Para aplicativos que não aceitam um usuário conectado, as permissões podem ser previamente autorizadas por um administrador quando o aplicativo é instalado.

### <a name="best-practices-for-requesting-permissions"></a>Práticas recomendadas para solicitar permissões
[!INCLUDE [auth-use-least-privileged](../../includes/auth-use-least-privileged.md)]

### <a name="delegated-and-application-permissions"></a>Permissões delegadas e de aplicativo
O Microsoft Graph tem dois tipos de permissões:

- As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente. Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo pode agir como o usuário conectado ao fazer chamadas ao Microsoft Graph. Algumas permissões delegadas podem ser autorizadas por usuários não administradores, mas algumas permissões com maiores privilégios exigem o [consentimento do administrador](/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint).  

- As **permissões de aplicativo** são usadas por aplicativos sem um usuário conectado; por exemplo, aplicativos executados como daemons ou serviços em segundo plano. As permissões de aplicativo só podem ser [autorizadas por um administrador](/azure/active-directory/develop/active-directory-v2-scopes#requesting-consent-for-an-entire-tenant). 

As _permissões efetivas_ são as permissões que seu aplicativo terá ao fazer solicitações ao Microsoft Graph. É importante compreender a diferença entre as Permissões Delegadas e as Permissões de aplicativo que o aplicativo tem autorização para usar e as respectivas Permissões Efetivas ao fazer chamadas para o Microsoft Graph

- No caso de permissões delegadas, as permissões efetivas do aplicativo estarão na interseção menos privilegiada das permissões delegadas que o aplicativo recebeu (por meio de consentimento) e dos privilégios do usuário atualmente conectado. O aplicativo jamais pode ter mais privilégios do que o usuário conectado. Nas organizações, os privilégios do usuário conectado podem ser determinados por uma política ou pela associação a uma ou mais funções de administrador. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).<br/><br/>Por exemplo, digamos que o aplicativo recebeu a Permissão Delegada User.ReadWrite.All. Essa permissão autoriza o aplicativo a ler e atualizar o perfil de todos os usuários em uma organização. Se o usuário conectado for um administrador global, seu aplicativo conseguirá atualizar o perfil de todos os usuários na organização. No entanto, se o usuário conectado não tiver uma função de administrador, seu aplicativo conseguirá atualizar apenas o perfil do usuário conectado. Ele não conseguirá atualizar os perfis de outros usuários na organização porque o usuário que tem permissão para agir em nome de outra pessoa não tem esses privilégios.
- No caso de Permissões de aplicativo, as Permissões Efetivas do aplicativo estarão no nível completo de privilégios implícitos da permissão. Por exemplo, um aplicativo que tem a Permissão de aplicativo User.ReadWrite.All pode atualizar o perfil de todos os usuários na organização.

>**Observação** Por padrão, os aplicativos que receberam permissões de aplicativo para os seguintes conjuntos de dados podem acessar todas as caixas de correio na organização:

- [Calendários](../permissions-reference.md#calendars-permissions)
- [Contatos](../permissions-reference.md#contacts-permissions)
- [Email](../permissions-reference.md#mail-permissions)
- [Configurações da Caixa de Correio](../permissions-reference.md#mail-permissions)

>Os administradores podem configurar a [política de acesso a aplicativos](../auth-limit-mailbox-access.md) para limitar o acesso do aplicativo a caixas de correio _específicas_.

Para obter uma lista completa das permissões do Microsoft Graph e saber quais permissões precisam de autorização de um administrador, confira a [Referência de permissões](../permissions-reference.md).

## <a name="getting-an-access-token"></a>Obter um token de acesso

Como a maioria dos desenvolvedores, você provavelmente usará bibliotecas de autenticação para gerenciar suas interações de token com a plataforma de identidade da Microsoft. As bibliotecas de autenticação abstraem muitos detalhes de protocolo (como validação, manipulação de cookies, cache de token e manutenção de conexões seguras) para longe do desenvolvedor e permitem que você foque no desenvolvimento do aplicativo. A Microsoft publica bibliotecas de cliente de código aberto e middleware de servidor.

Sobre o ponto de extremidade da Microsoft Identity Platform:

- As bibliotecas de cliente da Biblioteca de Autenticação da Microsoft (MSAL) estão disponíveis para .NET, JavaScript, Android e Objective-c. Todas as plataformas estão em pré-visualização com suporte à produção e, no caso de alterações serem introduzidas, a Microsoft garante um caminho para a atualização.
- O middleware de servidor da Microsoft está disponível para .NET core e ASP.NET (OWIN OpenID Connect e OAuth) e para Node.js (Microsoft Identity Platform Passport.js).
- A Microsoft Identity Platform é compatível com várias bibliotecas de autenticação de terceiros.

Para obter uma lista completa de bibliotecas de cliente da Microsoft, middleware de servidor da Microsoft e bibliotecas de terceiros compatíveis, confira [Bibliotecas de autenticação da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-v2-libraries).

Não é necessário usar uma biblioteca de autenticação para obter um token de acesso. Para saber mais sobre o uso direto dos pontos de extremidade da plataforma de identidade da Microsoft sem precisar de uma biblioteca de autenticação, confira [Autenticação da plataforma de identidade da Microsoft](/azure/active-directory/develop/authentication-scenarios).

## <a name="next-steps"></a>Próximas etapas

- Para etapas rápidas sobre a obtenção de token de acesso para aplicativos que fizerem chamadas para o Microsoft Graph, escolha o tipo de aplicativo adequado ao seu cenário:
  - [Aplicativo da área de trabalho](/azure/active-directory/develop/scenario-desktop-overview)
  - [Aplicativo móvel](/azure/active-directory/develop/scenario-mobile-overview)
  - [Aplicativo Web](/azure/active-directory/develop/scenario-web-app-call-api-overview)
  - [Aplicativo de página única](/azure/active-directory/develop/scenario-spa-overview)
  - [Daemon / serviços do plano de fundo](/azure/active-directory/develop/scenario-daemon-overview)
- Para ver as permissões que você pode usar com o Microsoft Graph, confira [Permissões](../permissions-reference.md).
- Se você é um provedor de Soluções na Nuvem da Microsoft interessado em acessar dados de clientes gerenciados por parceiros por meio do Microsoft Graph, confira [Gerenciar o acesso ao aplicativo (CSPs)](../auth-cloudsolutionprovider.md).

Se já estiver pronto para entrar no código, você pode usar os seguintes recursos para ajudá-lo a implementar a autenticação e a autorização com a Microsoft Identity Platform em seu aplicativo.

### <a name="microsoft-graph-training-and-samples"></a>Exemplos e treinamento do Microsoft Graph

Para ajudá-lo a começar rapidamente, criamos uma série de módulos de treinamento e outros recursos que mostram como autenticar e usar a API em diversas plataformas.

- Use a página [Introdução](https://developer.microsoft.com/graph/get-started) para encontrar bibliotecas, exemplos, conteúdo de treinamento e outros recursos para sua plataforma favorita.
- Para começar a trabalhar rapidamente com um exemplo pré-configurado para sua plataforma, confira o [Início Rápido do Microsoft Graph](https://developer.microsoft.com/graph/quick-start).
- Veja nossos [exemplos do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=) no GitHub.

### <a name="microsoft-identity-platform-samples-and-documentation"></a>Documentação e exemplos da Microsoft Identity Platform

A documentação da Microsoft Identity Platform contém artigos e exemplos que se concentram especificamente na autenticação e autorização com a Microsoft Identity Platform.

- A [documentação do ponto de extremidade da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-appmodel-v2-overview) é o melhor local para começar. Este artigo contém links para visualizações, documentação de protocolos e artigos de introdução para plataformas diferentes, todos organizados pelo tipo de aplicativo que você está desenvolvendo.
- Para exemplos de uso da plataforma de identidade da Microsoft para garantir diferentes tipos de aplicativos, confira [Exemplos de código da plataforma de identidade da Microsoft (ponto de extremidade v2.0)](/azure/active-directory/develop/sample-v2-code).
- Para ver exemplos listados pela biblioteca de autenticação de cliente ou servidor, confira [Bibliotecas de Autenticação da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-v2-libraries).
- Explore os exemplos por plataforma da Microsoft Identity Platform na [Galeria de código Azure](https://azure.microsoft.com/resources/samples/?service=active-directory).

## <a name="see-also"></a>Confira também

- [Escolher um provedor de autenticação do Microsoft Graph com base no cenário](../sdks/choose-authentication-providers.md)
- [Documentação do ponto de extremidade da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-appmodel-v2-overview)
