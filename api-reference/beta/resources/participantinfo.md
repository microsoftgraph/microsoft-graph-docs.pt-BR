---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568563"
---
# <a name="participantinfo-resource-type"></a>tipo de recurso participantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição  |
|:---------------|:------------------------------|:-------------|
| ladrões       | [identitySet](identityset.md) | O [identityset](identityset.md) associado a este participante. |
| languageId     | String                        | A cadeia de caracteres de cultura do idioma. |
| região         | String                        | Região do participante. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
