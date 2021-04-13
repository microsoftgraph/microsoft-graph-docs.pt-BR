---
title: Tipo de recurso channelIdentity
description: Representa a identidade de um canal no Microsoft Teams.
author: Kanaka
doc_type: resourcePageType
localization_priority: Normal
ms.prod: teamwork
ms.openlocfilehash: eae8533f549ba0064d9d392fcf60a5baa6479e2c
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697913"
---
# <a name="channelidentity-resource-type"></a>Tipo de recurso channelIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Contém informações básicas de identificação sobre um canal no Microsoft Teams.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|channelId|string|  A identidade do canal no qual a mensagem foi postada.|
|teamId|string|  A identidade da equipe na qual a mensagem foi postada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.channelIdentity"
}-->

```json
{
   "channelId":"string",
   "teamId":"string"
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
