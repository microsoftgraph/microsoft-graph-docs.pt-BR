---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1dcc164769c2e8168be5f593c35cd62218254add
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870985"
---
# <a name="participantinfo-resource-type"></a>tipo de recurso participantInfo

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| ladrões       | [identitySet](identityset.md) | O [identityset](identityset.md) associado a este participante. Somente leitura.                                                                             |
| languageId     | String                        | A cadeia de caracteres de cultura do idioma. Somente leitura.                                                                                                                    |
| região         | String                        | A região de início do participante. Pode ser um país, um continente ou uma região geográfica maior. Isso não é alterado com base no local físico atual do participante. Somente leitura. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
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
