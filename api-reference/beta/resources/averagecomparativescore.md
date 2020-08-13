---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e051ee3d1265c1dc65a5ab0cb9352d9cd536b21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508049"
---
#  <a name="averagecomparativescore-resource-type"></a>tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   String  |   Tipo de escopo (por islocatários, TotalSeats, IndustryTypes).  |
|   averageScore    |   Duplo  | Pontuação média dentro da base especificada. |
|   deviceScore |   Duplo  | Pontuação média dentro da base especificada. |
|   datascore   |   Duplo  | Pontuação média dentro da base especificada. |
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
