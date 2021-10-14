---
title: Tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f6c759ba3936d500b34566ac894895ce7b0f7ff7
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289851"
---
# <a name="participantinfo-resource-type"></a>Tipo de recurso participantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                            | Descrição                                                                                                                                                                                                      |
| :--------------- | :------------------------------ | :-----------------------------------------------------------------------------------------------------------------------------------------------------------                                                     |
| countryCode      | String                          | O código de país alpha-2 iso 3166-1 do local físico mais estimado do participante no início da chamada. Apenas leitura.                                                                                   |
| endpointType     | String                          | O tipo de ponto de extremidade que o participante está usando. Os valores possíveis são: `default`, `skypeForBusiness` ou `skypeForBusinessVoipPhone`. Apenas leitura.                                                                    |
| identity         | [identitySet](identityset.md)   | O [identitySet](identityset.md) associado a esse participante. Somente leitura.                                                                                                                                   |
| languageId       | String                          | A cadeia de caracteres de cultura de idioma. Apenas leitura.                                                                                                                                                                          |
| region           | String                          | A região 1 do participante. Pode ser um país, um continente ou uma região geográfica maior. Isso não muda com base na localização física atual do participante, ao contrário de countryCode. Apenas leitura. |
| platformId       | String                          | A ID da plataforma do cliente do participante. Apenas leitura.    |
| participantId    | String                          | A ID do participante. Somente leitura.    |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region",
    "platformId",
    "participantId"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
  "languageId": "String",
  "region": "String",
  "platformId": "String",
  "participantId": "String"
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


