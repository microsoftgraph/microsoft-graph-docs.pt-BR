---
title: tipo de recurso onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff5ca6afc76ab60ab82f045d0309832e34e8d708
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840765"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso onPremisesPublishing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto **onPremisesPublishing** representa o conjunto de propriedades para publicar o [aplicativo](application.md)local.

## <a name="properties"></a>Propriedades

| Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. Nulo ao usar o domínio padrão.|
|externalAuthenticationType|String|Detalhes a configuração de pré-autenticação para o aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|A URL externa publicada para o aplicativo. Por exemplohttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|A URL interna do aplicativo. Por exemplohttps://intranet/ |
|isOnPremPublishingEnabled|Booliano|Indica se o aplicativo está sendo publicado ou não no momento.|
|applicationServerTimeout|String|A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão. Os valores possíveis `default`são `long`:. Use `long` se o servidor levar mais de 60-75 segundos para responder às solicitações. Além disso `long` , tente se você não consegue acessar o aplicativo e o status do erro é "tempo limite de backend".|
|isTranslateHostHeaderEnabled|Booliano|Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta. Isso inclui a configuração do site correto para cookies.|

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
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
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
