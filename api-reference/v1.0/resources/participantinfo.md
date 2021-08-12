---
title: Tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2804e846b95f2aad597699b4799c280101b07e9a4bea9ae5413aefade1d5c984
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146437"
---
# <a name="participantinfo-resource-type"></a>Tipo de recurso participantInfo

Namespace: microsoft.graph

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | Cadeia de caracteres                        | O código de país alpha-2 iso 3166-1 do local físico mais estimado do participante no início da chamada. Somente leitura.                             |
| endpointType   | Cadeia de caracteres                        | O tipo de ponto de extremidade que o participante está usando. Os valores possíveis são: `default`, `skypeForBusiness` ou `skypeForBusinessVoipPhone`. Apenas leitura.              |
| identity       | [identitySet](identityset.md) | O [identitySet](identityset.md) associado a esse participante. Somente leitura.                                                                             |
| languageId     | String                        | A cadeia de caracteres de cultura de idioma. Somente leitura.                                                                                                                    |
| region         | Cadeia de caracteres                        | A região 1 do participante. Pode ser um país, um continente ou uma região geográfica maior. Isso não muda com base no local físico atual do participante. Somente leitura. |


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

