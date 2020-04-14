---
title: tipo de recurso accessReviewRecurrenceSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7c45a0b57d869acdb49c5a37f235232c70e8ec6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472233"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>tipo de recurso accessReviewRecurrenceSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| recurrenceType | cadeia de caracteres |  |
| recurrenceEndType | cadeia de caracteres |  |
| durationInDays | Int32 |  |
| recurrenceCount | Int32 |  |

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



