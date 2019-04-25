---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535435"
---
#  <a name="averagecomparativescore-resource-type"></a>tipo de recurso averageComparativeScore

Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   String  |   Tipo de escopo (por isLocatários, TotalSeats, IndustryTypes).  |
|   averageScore    |   Duplo  | Pontuação média dentro da base especificada. |
|   deviceScore |   Duplo  | Pontuação média dentro da base especificada. |
|   dataScore   |   Duplo  | Pontuação média dentro da base especificada. |
|   identityScore   |   Duplo  | Pontuação média dentro da base especificada. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
