---
title: Tipo de recurso onPremisesPublishing
description: Representa um objeto Application Proxy onPremisesPublishing.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5b884d6f1aadb43d682cba1434ed4d31e0ae1e70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956922"
---
# <a name="onpremisespublishing-resource-type"></a>Tipo de recurso onPremisesPublishing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um aplicativo local publicado por meio do Proxy de Aplicativo [do Azure AD](https://aka.ms/whyappproxy) é representado por um objeto [de](application.md) aplicativo e sua propriedade **onPremisesPublishing** associada. O Proxy de Aplicativo fornece acesso remoto seguro a aplicativos locais.

Um **objeto onPremisesPublishing** representa o conjunto de propriedades para configurar o Proxy de Aplicativo para um aplicativo [local.](application.md) 

Depois [de instautar](../api/applicationtemplate-instantiate.md) um aplicativo personalizado ou criar um [aplicativo,](../api/application-post-applications.md)as configurações de Proxy de Aplicativo para o aplicativo podem ser configuradas atualizando as propriedades onPremisesPublishing do aplicativo. [](../api/application-update.md)

Para um tutorial sobre como configurar o Proxy de Aplicativo, consulte [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).

## <a name="properties"></a>Propriedades

| Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|alternateUrl|Cadeia de caracteres| Se você estiver configurando um gerenciador de tráfego na frente de vários aplicativos proxy de aplicativo, o alternateUrl será a URL amigável que apontará para o gerente de tráfego. |
|applicationServerTimeout|Cadeia de caracteres| A duração que o conector aguardará por uma resposta do aplicativo back-end antes de fechar a conexão. Os valores possíveis `default` são , `long` . Quando definido como padrão, o tempo decoro do aplicativo back-end tem um comprimento de 85 segundos. Quando definido como longo, o tempo de tempo de back-end é aumentado para 180 segundos. Use se o servidor levar mais de 85 segundos para responder a solicitações ou se você não conseguir acessar o aplicativo e o status do erro for "Tempo de tempo de `long` back-end". O valor padrão é `default`. |
|applicationType|Cadeia de caracteres| Indica se esse aplicativo é um aplicativo configurado para Proxy de Aplicativo. Isso é pré-definido pelo sistema. Somente leitura. |
|externalAuthenticationType|externalAuthenticationType| Detalha a configuração de pré-autenticação do aplicativo. A pré-autenticação impõe que os usuários devem autenticar antes de acessar o aplicativo. Passthru não exige autenticação. Os valores possíveis são: `passthru` e `aadPreAuthentication`. |
|externalUrl|Cadeia de caracteres| A URL externa publicada para o aplicativo. Por exemplo, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|Cadeia de caracteres| A URL interna do aplicativo. Por exemplo, https://intranet/. |
|éHttpOnlyCookieEnabled|Booliano| Indica se o sinalizador de cookie HTTPOnly deve ser definido nos cabeçalhos de resposta HTTP. De definir esse valor para que os cookies de Proxy de `true` Aplicativo incluam o sinalizador HTTPOnly nos cabeçalhos de resposta HTTP. Se estiver usando os Serviços de Área de Trabalho Remota, de definir esse valor como False. O valor padrão é `false`. |
|isOnPremPublishingEnabled|Booliano| Indica se o aplicativo está sendo publicado por meio do Proxy de Aplicativo ou não. Isso é pré-definido pelo sistema. Somente leitura. |
|isPersistentCookieEnabled|Booliano| Indica se o sinalizador de cookie persistente deve ser definido nos cabeçalhos de resposta HTTP. Mantenha esse valor definido como `false` . Use essa configuração apenas para aplicativos que não podem compartilhar cookies entre processos. Para obter mais informações sobre configurações de cookie, consulte Configurações de cookie para acessar aplicativos locais [no Azure Active Directory](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings). O valor padrão é `false`. |
|isSecureCookieEnabled|Booliano| Indica se o sinalizador de cookie seguro deve ser definido nos cabeçalhos de resposta HTTP. De definir esse valor `true` para transmitir cookies por um canal seguro, como uma solicitação HTTPS criptografada. O valor padrão é `true`.|
|isTranslateHostHeaderEnabled|Booliano| Indica se o aplicativo deve traduzir urls nos headers de reponse. Mantenha esse valor como `true` a menos que seu aplicativo exigiu o header de host original na solicitação de autenticação. O valor padrão é `true`.|
|isTranslateLinksInBodyEnabled|Booliano| Indica se o aplicativo deve traduzir urls no corpo do aplicativo. Mantenha esse valor como, a menos que você tenha links HTML decodificados para outros aplicativos locais e `false` não use domínios personalizados. Para obter mais informações, [consulte Link translation with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation). O valor padrão é `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Representa a configuração de entrada única para o aplicativo local. |
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


