---
title: Tipo de recurso onPremisesPublishing
description: Representa um objeto Application Proxy onPremisesPublishing .
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74ecc94c88990b042e35a7a2701d7a1cd50b1199
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134880"
---
# <a name="onpremisespublishing-resource-type"></a>Tipo de recurso onPremisesPublishing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um aplicativo local publicado por meio do Proxy de Aplicativo [](application.md) do [Azure AD](https://aka.ms/whyappproxy) é representado por um objeto de aplicativo e sua propriedade **onPremisesPublishing** associada. O Proxy de Aplicativo fornece acesso remoto seguro a aplicativos locais.

Um **objeto onPremisesPublishing** representa o conjunto de propriedades para configurar o Proxy de Aplicativo para um aplicativo [local.](application.md) 

Depois [de inciar](../api/applicationtemplate-instantiate.md) um aplicativo personalizado ou criar um [aplicativo,](../api/application-post-applications.md)as configurações do Proxy de Aplicativo para o aplicativo podem ser configuradas atualizando as propriedades de publicação onPremises do aplicativo. [](../api/application-update.md)

Para um tutorial sobre como configurar o Proxy de Aplicativo, confira Automatizar a configuração do Proxy de Aplicativo usando a [API do Microsoft Graph.](/graph/application-proxy-configure-api)

## <a name="properties"></a>Propriedades

| Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|alternateUrl|String| Se você estiver configurando um gerenciador de tráfego na frente de vários aplicativos de Proxy de Aplicativo, a alternateUrl será a URL amigável que apontará para o gerenciador de tráfego. |
|applicationServerTimeout|String| A duração que o conector aguardará por uma resposta do aplicativo back-end antes de fechar a conexão. Os valores possíveis `default` são , `long` . Quando definido como padrão, o tempo máximo do aplicativo back-end tem um comprimento de 85 segundos. Quando definido como longo, o tempo de tempo de back-back é aumentado para 180 segundos. Use se o servidor levar mais de 85 segundos para responder a solicitações ou se você não conseguir acessar o aplicativo e o status do erro for `long` "Backend Timeout". O valor padrão é `default`. |
|applicationType|Cadeia de caracteres| Indica se esse aplicativo é um aplicativo configurado para Proxy de Aplicativo. Isso é pré-definido pelo sistema. Somente leitura. |
|externalAuthenticationType|String| Detalha a configuração de pré-autenticação do aplicativo. A pré-autenticação impõe que os usuários devem autenticar antes de acessar o aplicativo. Passthru não requer autenticação. Os valores possíveis são: `passthru` e `aadPreAuthentication`. |
|externalUrl|String| A URL externa publicada para o aplicativo. Por exemplo, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|String| A URL interna do aplicativo. Por exemplo, https://intranet/. |
|isHttpOnlyCookieEnabled|Boolean| Indica se o sinalizador de cookie HTTPOnly deve ser definido nos cabeçalhos de resposta HTTP. De definir esse valor para que os cookies do Proxy de Aplicativo incluam o sinalizador `true` HTTPOnly nos cabeçalhos de resposta HTTP. Se estiver usando os Serviços de Área de Trabalho Remota, de definida como False. O valor padrão é `false`. |
|isOnPremPublishingEnabled|Boolean| Indica se o aplicativo está sendo publicado por meio do Proxy de Aplicativo ou não. Isso é pré-definido pelo sistema. Somente leitura. |
|isPersistentCookieEnabled|Boolean| Indica se o sinalizador de cookie persistente deve ser definido nos cabeçalhos de resposta HTTP. Mantenha esse valor definido como `false` . Use essa configuração somente para aplicativos que não podem compartilhar cookies entre processos. Para obter mais informações sobre configurações de cookie, consulte Configurações de cookie para acessar aplicativos locais [no Azure Active Directory.](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings) O valor padrão é `false`. |
|isSecureCookieEnabled|Boolean| Indica se o sinalizador de cookie seguro deve ser definido nos cabeçalhos de resposta HTTP. De configurar esse valor `true` para transmitir cookies por um canal seguro, como uma solicitação HTTPS criptografada. O valor padrão é `true`.|
|isTranslateHostHeaderEnabled|Boolean| Indica se o aplicativo deve traduzir URLs nos títulos de reponse. Mantenha esse valor, a `true` menos que seu aplicativo tenha exigido o título de host original na solicitação de autenticação. O valor padrão é `true`.|
|isTranslateLinksInBodyEnabled|Boolean| Indica se o aplicativo deve traduzir URLs no corpo do aplicativo. Mantenha esse valor como a menos que você tenha links HTML em código para outros aplicativos locais e não `false` use domínios personalizados. Para obter mais informações, consulte [Link translation with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation). O valor padrão é `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Representa a configuração de login único para o aplicativo local. |
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
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
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


