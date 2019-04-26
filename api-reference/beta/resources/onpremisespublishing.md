---
title: tipo de recurso onPremisesPublishing
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341772"
---
# <a name="onpremisespublishing-resource-type"></a>tipo de recurso onPremisesPublishing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customDomainCertificate|String|Detalhes do certificado associado ao aplicativo quando um domínio personalizado está em uso. Nulo ao usar o domínio padrão.|
|externalAuthenticationType|String|Detalhes a configuração de pré-autenticação para o aplicativo os valores possíveis são: `passthru`, `aadPreAuthentication`.|
|externalUrl|String|A URL externa publicada para o aplicativo. Por exemplohttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|A URL interna do aplicativo. Por exemplohttps://intranet/ |
|isOnPremPublishingEnabled|Boolean|Indica se o aplicativo está sendo publicado ou não no momento.|
|applicationServerTimeout|String|A duração que o conector aguardará por uma resposta do aplicativo backend antes de fechar a conexão. Os valores possíveis `default`são `long`:. Use `long` se o servidor levar mais de 60-75 segundos para responder às solicitações. Além disso `long` , tente se você não consegue acessar o aplicativo e o status do erro é "tempo limite de backend".|
|isTranslateHostHeaderEnabled|Boolean|Indica se o aplicativo deve traduzir URLs nos cabeçalhos de resposta. Isso inclui a configuração do site correto para cookies.|

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
2015-10-25 14:57:30 UTC -->
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
