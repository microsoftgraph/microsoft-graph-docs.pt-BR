---
title: tipo de recurso resourceAccess
description: Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo. A propriedade **resourceAccess** do tipo requiredResourceAccess é uma coleção de **resourceAccess**.
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343630"
---
# <a name="resourceaccess-resource-type"></a>tipo de recurso resourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica um escopo de permissão OAuth 2,0 ou uma função de aplicativo exigida por um aplicativo. A propriedade **resourceAccess** do tipo [requiredResourceAccess](requiredresourceaccess.md) é uma coleção de **resourceAccess**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Guid|O identificador exclusivo de uma das instâncias [oAuth2Permission](oauth2permission.md) ou [appRole](approle.md) que o aplicativo de recursos expõe.|
|type|String|Especifica se a propriedade **ID** faz referência a um [OAuth2Permission](oauth2permission.md) ou um [appRole](approle.md). Os valores possíveis são "escopo" ou "função".|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
