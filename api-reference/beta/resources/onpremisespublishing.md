---
title: tipo de recurso onPremisesPublishing
description: Representa um objeto de onPremisesPublishing do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4d19a726e2f09c1df994bc8aee7d91eb53ef2628
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682002"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso onPremisesPublishing

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um aplicativo local publicado por meio [do proxy de aplicativo do Azure ad](https://aka.ms/whyappproxy) é representado por um objeto [Application](application.md) e sua propriedade **onPremisesPublishing** associada. O proxy de aplicativo fornece acesso remoto seguro a aplicativos locais.

Um objeto **onPremisesPublishing** representa o conjunto de propriedades para configurar o proxy de aplicativo para um [aplicativo](application.md)local. 

Após [instanciar um aplicativo personalizado](../api/applicationtemplate-instantiate.md) ou [criar um aplicativo](../api/application-post-applications.md), as configurações de proxy do aplicativo para o aplicativo podem ser configuradas [atualizando as](../api/application-update.md) Propriedades de onPremisesPublishing do aplicativo.

## <a name="properties"></a>Propriedades

| Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|alternateUrl|String| Se você estiver configurando um gerente de tráfego na frente de vários aplicativos de proxy de aplicativo, o alternateUrl será a URL amigável para o usuário que apontará para o Gerenciador de tráfego. |
|applicationServerTimeout|String| A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão. Os valores possíveis são `default` : `long` . Quando definido como padrão, o tempo limite do aplicativo de back-end tem um tamanho de 85 segundos. Quando definido como Long, o tempo limite de back-end é aumentado para 180 segundos. Use `long` se o servidor levar mais de 85 segundos para responder às solicitações ou se você não conseguir acessar o aplicativo e o status de erro for "tempo limite de back-end". O valor padrão é `default`. |
|applicationType|Cadeia de caracteres| Indica se este aplicativo é um aplicativo configurado de proxy de aplicativo. Isso é predefinido pelo sistema. Somente leitura. |
|externalAuthenticationType|String| Detalha a configuração de pré-autenticação para o aplicativo. A pré-autenticação impõe que os usuários devem se autenticar antes de acessar o aplicativo. PassThru não requer autenticação. Os valores possíveis são: `passthru` e `aadPreAuthentication`. |
|externalUrl|String| A URL externa publicada para o aplicativo. Por exemplo, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|String| A URL interna do aplicativo. Por exemplo, https://intranet/. |
|isHttpOnlyCookieEnabled|Booliano| Indica se o sinalizador de cookie HTTPOnly deve ser definido nos cabeçalhos de resposta HTTP. Defina esse valor como `true` para que os cookies de proxy do aplicativo incluam o sinalizador HTTPOnly nos cabeçalhos de resposta http. Se estiver usando os serviços de área de trabalho remota, defina esse valor como false. O valor padrão é `false`. |
|isOnPremPublishingEnabled|Booliano| Indica se o aplicativo está sendo publicado no momento por meio do proxy de aplicativo ou não. Isso é predefinido pelo sistema. Somente leitura. |
|isPersistentCookieEnabled|Booliano| Indica se o sinalizador de cookie persistente deve ser definido nos cabeçalhos de resposta HTTP. Mantenha este valor definido como `false` . Use essa configuração apenas para aplicativos que não podem compartilhar cookies entre processos. Para obter mais informações sobre configurações de cookie, consulte [configurações de cookie para acessar aplicativos locais no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings). O valor padrão é `false`. |
|isSecureCookieEnabled|Booliano| Indica se o sinalizador de cookie seguro deve ser definido nos cabeçalhos de resposta HTTP. Defina esse valor como `true` para transmitir cookies por meio de um canal seguro, como uma solicitação HTTPS criptografada. O valor padrão é `true`.|
|isTranslateHostHeaderEnabled|Booliano| Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta. Mantenha esse valor como `true` a menos que seu aplicativo requerido o cabeçalho de host original na solicitação de autenticação. O valor padrão é `true`.|
|isTranslateLinksInBodyEnabled|Booliano| Indica se o aplicativo deve traduzir URLs no corpo do aplicativo. Mantenha esse valor como `false` a menos que você tenha links HTML codificados para outros aplicativos locais e não use domínios personalizados. Para obter mais informações, consulte [conversão de link com o proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation). O valor padrão é `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Representa a configuração de logon único para o aplicativo local. |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. `null`ao usar o domínio padrão. Somente leitura.|
|verifiedCustomDomainKeyCredential|[keycredential](keycredential.md)| A credencial de chave associada para o domínio personalizado usado. |
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
