---
title: Tipo de recurso participantInfo
description: Contém propriedades adicionais sobre a identidade do participante
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1d134eec6e6bef50eb7a97917a2f8aaa3b91148
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104072"
---
# <a name="participantinfo-resource-type"></a>Tipo de recurso participantInfo

Namespace: microsoft.graph

Contém propriedades adicionais sobre a identidade do participante

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| countryCode    | String                        | O código de país alpha-2 iso 3166-1 do local físico mais estimado do participante no início da chamada. Somente leitura.                             |
| endpointType   | String                        | O tipo de ponto de extremidade que o participante está usando. Os valores possíveis são: `default`, `skypeForBusiness` ou `skypeForBusinessVoipPhone`. Somente leitura.              |
| identity       | [identitySet](identityset.md) | O [identitySet](identityset.md) associado a esse participante. Somente leitura.                                                                             |
| languageId     | String                        | A cadeia de caracteres de cultura de idioma. Somente leitura.                                                                                                                    |
| region         | String                        | A região 1 do participante. Pode ser um país, um continente ou uma região geográfica maior. Isso não muda com base no local físico atual do participante. Somente leitura. |


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

