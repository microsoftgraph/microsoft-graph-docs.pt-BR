---
title: Tipo de recurso onPremisesPublishing
description: Representa um Proxy de Aplicativo objeto onPremisesPublishing.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 453bf7f0ab0f0d13e5c333375d74518251b3f115
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246787"
---
# <a name="onpremisespublishing-resource-type"></a>Tipo de recurso onPremisesPublishing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um aplicativo local publicado via [Azure AD Proxy de Aplicativo](/azure/active-directory/app-proxy/what-is-application-proxy) é representado por um objeto de aplicativo e sua propriedade **onPremisesPublishing** associada.[](application.md) Proxy de Aplicativo fornece acesso remoto seguro a aplicativos locais.

Um **objeto onPremisesPublishing** representa o conjunto de propriedades para Proxy de Aplicativo para um aplicativo [local](application.md). 

Depois [de criar](../api/applicationtemplate-instantiate.md) uma instância de um aplicativo personalizado ou criar um [aplicativo, as](../api/application-post-applications.md) Proxy de Aplicativo configurações do aplicativo podem ser definidas atualizando as [propriedades onPremisesPublishing](../api/application-update.md) do aplicativo.

Para obter um tutorial sobre como Proxy de Aplicativo, consulte Automatizar a configuração de Proxy de Aplicativo [usando o Microsoft API do Graph](/graph/application-proxy-configure-api).

## <a name="properties"></a>Propriedades

| Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|Alternateurl|Cadeia de caracteres| Se você estiver configurando um gerenciador de tráfego na frente de vários aplicativos de Proxy de Aplicativo, a alternateUrl será a URL amigável que apontará para o gerenciador de tráfego. |
|applicationServerTimeout|Cadeia de caracteres| A duração que o conector aguardará por uma resposta do aplicativo de back-end antes de fechar a conexão. Os valores possíveis são `default`, `long`. Quando definido como padrão, o tempo limite do aplicativo de back-end tem um comprimento de 85 segundos. Quando definido como longo, o tempo limite de back-end é aumentado para 180 segundos. Use `long` se o servidor levar mais de 85 segundos para responder às solicitações ou se você não conseguir acessar o aplicativo e o status do erro for "Tempo limite de back-end". O valor padrão é `default`. |
|applicationType|Cadeia de caracteres| Indica se esse aplicativo é um Proxy de Aplicativo configurado. Isso é pré-definido pelo sistema. Somente leitura. |
|externalAuthenticationType|externalAuthenticationType| Detalha a configuração de pré-autenticação do aplicativo. A pré-autenticação impõe que os usuários devem se autenticar antes de acessar o aplicativo. Passthru não requer autenticação. Os valores possíveis são: `passthru` e `aadPreAuthentication`. |
|Externalurl|Cadeia de caracteres| A URL externa publicada para o aplicativo. Por exemplo, https://intranet-contoso.msappproxy.net/.  |
|Internalurl|Cadeia de caracteres| A URL interna do aplicativo. Por exemplo, https://intranet/. |
|isBackendCertificateValidationEnabled|Booliano| Indica se a validação do certificado SSL de back-end está habilitada para o aplicativo. Para todos os Proxy de Aplicativo novos aplicativos, a propriedade será definida como `true` por padrão. Para todos os aplicativos existentes, a propriedade será definida como `false`. |
|isHttpOnlyCookieEnabled|Booliano| Indica se o sinalizador de cookie HTTPOnly deve ser definido nos cabeçalhos de resposta HTTP. Defina esse valor para `true` que Proxy de Aplicativo cookies incluam o sinalizador HTTPOnly nos cabeçalhos de resposta HTTP. Se estiver usando os Serviços de Área de Trabalho Remota, defina esse valor como False. O valor padrão é `false`. |
|isOnPremPublishingEnabled|Booliano| Indica se o aplicativo está sendo publicado por meio Proxy de Aplicativo ou não. Isso é pré-definido pelo sistema. Somente leitura. |
|isPersistentCookieEnabled|Booliano| Indica se o sinalizador de cookie persistente deve ser definido nos cabeçalhos de resposta HTTP. Mantenha esse valor definido como `false`. Use essa configuração somente para aplicativos que não podem compartilhar cookies entre processos. Para obter mais informações sobre configurações de cookie, consulte [Configurações de cookie para acessar aplicativos locais no Azure Active Directory](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings). O valor padrão é `false`. |
|isSecureCookieEnabled|Booliano| Indica se o sinalizador de cookie seguro deve ser definido nos cabeçalhos de resposta HTTP. Defina esse valor para `true` transmitir cookies por um canal seguro, como uma solicitação HTTPS criptografada. O valor padrão é `true`.|
|isStateSessionEnabled|Booliano| Indica se a validação do parâmetro de estado quando o cliente usa o fluxo de concessão de código de autorização OAuth 2.0 está habilitada. Essa configuração permite que os administradores especifiquem se querem habilitar a proteção CSRF para seus aplicativos. |
|isTranslateHostHeaderEnabled|Booliano| Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta. Mantenha esse valor como se `true` o aplicativo não exigia o cabeçalho de host original na solicitação de autenticação. O valor padrão é `true`.|
|isTranslateLinksInBodyEnabled|Booliano| Indica se o aplicativo deve traduzir URLs no corpo do aplicativo. Mantenha esse valor como a `false` menos que você tenha embutido links HTML em código para outros aplicativos locais e não use domínios personalizados. Para obter mais informações, consulte [Tradução de link com Proxy de Aplicativo](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation). O valor padrão é `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Representa a configuração de logon único para o aplicativo local. |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. `null` ao usar o domínio padrão. Somente leitura.|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| A credencial de chave associada para o domínio personalizado usado. |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| A credencial de senha associada para o domínio personalizado usado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "alternateUrl": "String",
  "applicationServerTimeout": "String",
  "applicationType": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isBackendCertificationValidationEnabled": true,
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
  "isStateSessionEnabled": true,
  "isTranslateHostHeaderEnabled": true,
  "isTranslateLinksInBodyEnabled": true,
  "singleSignOnSettings": {"@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"},
  "verifiedCustomDomainCertificatesMetadata": {"@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"},
  "verifiedCustomDomainKeyCredential": {"@odata.type": "microsoft.graph.keyCredential"},
  "verifiedCustomDomainPasswordCredential": {"@odata.type": "microsoft.graph.passwordCredential"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
