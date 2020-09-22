---
title: tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b48c8d9e8e2b7b39a63b919ff30178d8c8ac8536
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998240"
---
# <a name="participantinfo-resource-type"></a>tipo de recurso participantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | String                        | O código do país ISO 3166-1 alfa-2 do local físico mais estimado do participante no início da chamada. Somente leitura.                             |
| EndpointType   | String                        | O tipo de ponto de extremidade que o participante está usando. Os valores possíveis são: `default` , `skypeForBusiness` , ou `skypeForBusinessVoipPhone` . Somente leitura.              |
| ladrões       | [identitySet](identityset.md) | O [identityset](identityset.md) associado a este participante. Somente leitura.                                                                             |
| languageId     | String                        | A cadeia de caracteres de cultura do idioma. Somente leitura.                                                                                                                    |
| região         | String                        | A região de início do participante. Pode ser um país, um continente ou uma região geográfica maior. Isso não é alterado com base no local físico atual do participante, ao contrário do countryCode. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
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


