---
title: Princípios Básicos de Autenticação e Autorização para o Microsoft Graph
description: Para chamar o Microsoft Graph, o aplicativo deve adquirir um token de acesso da Microsoft Identity Plataform.
author: matt-steele
ms.localizationpriority: high
ms.prod: applications
ms.custom: graphiamtop20
ms.openlocfilehash: 3ac6d5ce6d6f1104f09faefcd06aaf1dd2b55422
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078573"
---
# <a name="authentication-and-authorization-basics-for-microsoft-graph"></a>Princípios Básicos de Autenticação e Autorização para o Microsoft Graph

Para chamar o Microsoft Graph, seu aplicativo deve adquirir um token de acesso da plataforma de identidade da Microsoft. O token de acesso contém informações sobre o aplicativo e as permissões que ele tem para os recursos e APIs disponíveis no Microsoft Graph. Para obter um token de acesso, o aplicativo deve ser registrado na plataforma de identidade da Microsoft e ter a autorização de um usuário ou administrador para acessar os recursos necessários do Microsoft Graph.

Este artigo fornece uma visão geral dos tokens de acesso, a plataforma de identidade da Microsoft e como seu aplicativo pode obter tokens de acesso. Se você sabe como integrar um aplicativo à plataforma de identidade da Microsoft para obter tokens, consulte as informações e amostras específicas do Microsoft Graph na seção [Passos seguintes](#next-steps).

## <a name="access-tokens"></a>Tokens de acesso

Os tokens de acesso emitidos pela plataforma de identidade da Microsoft contêm informações (declarações) que as APIs da web protegidas pela plataforma de identidade da Microsoft, como o Microsoft Graph, usam para validar o chamador e garantir que o chamador tenha as permissões adequadas para realizar a operação solicitada. Ao chamar o Microsoft Graph, trate os tokens de acesso como opacos. Sempre transmita tokens de acesso por um canal seguro, como o protocolo TLS (HTTPS).

O exemplo a seguir mostra um token de acesso à plataforma de identidade da Microsoft:

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
- **URI/URL de Redirecionamento**: um ou mais pontos de extremidade nos quais seu aplicativo receberá respostas da plataforma de identidade da Microsoft. (Para aplicativos nativos e móveis, este é um URI atribuído pela plataforma de identidade da Microsoft.)
- **Segredo do Aplicativo**: uma senha ou um par de chaves pública/privada que seu aplicativo usa para se autenticar na plataforma de identidade da Microsoft. (Não é necessário para aplicativos nativos ou móveis.)

As propriedades configuradas durante o registro são usadas na solicitação. Por exemplo, na seguinte solicitação de token: *client_id* é a *ID do Aplicativo*, *redirect_uri* é um dos *URIs de Redirecionamento* registrados do seu aplicativo e *client_secret* é o *Segredo do Aplicativo*.

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

- **Permissões delegadas** são usadas por aplicativos que possuem um usuário conectado presente. Para esses aplicativos, o usuário ou um administrador consente com as permissões que o aplicativo solicita e o aplicativo atua como o usuário conectado ao fazer chamadas para o Microsoft Graph. Algumas permissões delegadas podem ser consentidas por usuários não administrativos, mas algumas permissões mais privilegiadas requerem o [consentimento do administrador](/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint).  

- As **permissões de aplicativo** são usadas por aplicativos executados sem a presença de um usuário conectado; por exemplo, aplicativos executados como serviços ou daemons em segundo plano. As permissões do aplicativo só podem ser [autorizadas por um administrador](/azure/active-directory/develop/active-directory-v2-scopes#requesting-consent-for-an-entire-tenant). 

_Permissões efetivas_ são as permissões que seu aplicativo possui ao fazer solicitações ao Microsoft Graph. É importante entender a diferença entre as permissões delegadas e de aplicativo concedidas ao seu aplicativo e suas permissões efetivas ao fazer chamadas para o Microsoft Graph.

- Para permissões delegadas, as permissões efetivas de seu aplicativo são a interseção das permissões delegadas que o aplicativo recebeu (por meio de consentimento) e os privilégios do usuário conectado no momento. Seu aplicativo nunca pode ter mais privilégios do que o usuário conectado. Nas organizações, os privilégios do usuário conectado são determinados pela política ou pela associação a uma ou mais funções de administrador. Para obter mais informações sobre funções de administrador, confira [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles).<br/><br/>Por exemplo, suponha que seu aplicativo tenha recebido a permissão delegada *User.ReadWrite.All*. Essa permissão concede nominalmente ao seu aplicativo permissão para ler e atualizar o perfil de cada usuário em uma organização. Se o usuário conectado for um administrador global, seu aplicativo atualizará o perfil de cada usuário na organização. No entanto, se o usuário conectado não estiver em uma função de administrador, seu aplicativo poderá atualizar apenas o perfil do usuário conectado. Ele não atualizará os perfis de outros usuários na organização porque o usuário conectado não tem esses privilégios.

- Para permissões de aplicativo, as permissões efetivas do seu aplicativo estarão no nível completo de privilégios implícitos na permissão. Por exemplo, um aplicativo que tem a permissão de aplicativo *User.ReadWrite.All* pode atualizar o perfil de cada usuário na organização.

:::image type="content" source="/graph/images/auth-v2/permission-types.png" alt-text="O Microsoft Graph expõe as permissões delegadas e de aplicativo, mas autoriza solicitações com base nas permissões efetivas do aplicativo." border="true":::

>**Observação** Por padrão, os aplicativos que receberam permissões de aplicativo para os seguintes conjuntos de dados podem acessar todas as caixas de correio na organização:

- [Calendários](../permissions-reference.md#calendars-permissions)
- [Contatos](../permissions-reference.md#contacts-permissions)
- [Email](../permissions-reference.md#mail-permissions)
- [Configurações da Caixa de Correio](../permissions-reference.md#mail-permissions)

>Os administradores podem configurar a [política de acesso a aplicativos](../auth-limit-mailbox-access.md) para limitar o acesso do aplicativo a caixas de correio _específicas_.

Para uma lista completa das permissões delegadas e de aplicativos para o Microsoft Graph, e quais permissões exigem o consentimento do administrador, consulte a [Referência Permissões](../permissions-reference.md).

## <a name="getting-an-access-token"></a>Como obter um token de acesso

Como a maioria dos desenvolvedores, você provavelmente utilizará as bibliotecas de autenticação para gerenciar suas interações de token com a plataforma de identidade da Microsoft. Bibliotecas de autenticação abstraem muitos detalhes de protocolo, como validação, manipulação de cookies, cache de token e manutenção de conexões seguras, longe do desenvolvedor, e permitem que você concentre seu desenvolvimento no seu aplicativo. A Microsoft publica bibliotecas de cliente de código aberto e middleware de servidor.

Sobre o ponto de extremidade da plataforma de identidade para desenvolvedores da Microsoft:

- As bibliotecas de cliente da Biblioteca de Autenticação da Microsoft (MSAL) estão disponíveis para .NET, JavaScript, Android e Objective-C. Todas as plataformas estão em pré-visualização com suporte à produção e, caso alterações importantes sejam introduzidas, a Microsoft garante um caminho para a atualização.
- O middleware de servidor da Microsoft está disponível para .NET core e ASP.NET (OWIN OpenID Connect e OAuth) e para Node.js (Microsoft Identity Platform Passport.js).
- A Microsoft Identity Platform é compatível com várias bibliotecas de autenticação de terceiros.

Para obter uma lista completa de bibliotecas de cliente da Microsoft, middleware de servidor da Microsoft e bibliotecas de terceiros compatíveis, confira [Bibliotecas de autenticação da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-v2-libraries).

Você não precisa usar uma biblioteca de autenticação para obter um token de acesso. Para saber mais sobre o uso direto dos pontos de extremidade da plataforma de identidade da Microsoft sem precisar de uma biblioteca de autenticação, confira [Autenticação da plataforma de identidade da Microsoft](/azure/active-directory/develop/authentication-scenarios).

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

Para ajudá-lo a começar rapidamente, criamos uma série de módulos de treinamento e outros recursos que mostram como autenticar e usar a API em várias plataformas.

- Use a página [Introdução](https://developer.microsoft.com/graph/get-started) para encontrar bibliotecas, exemplos, conteúdo de treinamento e outros recursos para sua plataforma favorita.
- Para começar a trabalhar rapidamente com um exemplo pré-configurado para sua plataforma, confira o [Início Rápido do Microsoft Graph](https://developer.microsoft.com/graph/quick-start).
- Veja nossos [exemplos do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=) no GitHub.

### <a name="microsoft-identity-platform-samples-and-documentation"></a>Documentação e exemplos da Microsoft Identity Platform

A documentação da Microsoft Identity Platform contém artigos e exemplos que se concentram especificamente na autenticação e autorização com a Microsoft Identity Platform.

- O lugar mais fácil para começar é na [Documentação de ponto de extremidade da plataforma de identidade da Microsoft](/azure/active-directory/develop/active-directory-appmodel-v2-overview). Este artigo contém links para visões gerais, documentação de protocolo e artigos de introdução para diferentes plataformas, todos organizados pelo tipo de aplicativo que você está desenvolvendo.
- Para exemplos de uso da plataforma de identidade da Microsoft para garantir diferentes tipos de aplicativos, confira [Exemplos de código da plataforma de identidade da Microsoft (ponto de extremidade v2.0)](/azure/active-directory/develop/sample-v2-code).
- Para ver exemplos listados pela biblioteca de autenticação de cliente ou servidor, confira [Bibliotecas de Autenticação da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-v2-libraries).
- Explore os exemplos por plataforma da Microsoft Identity Platform na [Galeria de código Azure](https://azure.microsoft.com/resources/samples/?service=active-directory).

## <a name="see-also"></a>Confira também

- [Escolher um provedor de autenticação do Microsoft Graph com base no cenário](../sdks/choose-authentication-providers.md)
- [Documentação do ponto de extremidade da Microsoft Identity Platform](/azure/active-directory/develop/active-directory-appmodel-v2-overview)
