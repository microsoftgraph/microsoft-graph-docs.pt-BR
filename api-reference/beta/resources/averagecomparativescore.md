---
title: " tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho médio vertical da indústria, média por tamanho de assentos da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f2ac965d4dae0b038f3aad9fe13ed57a283a42bc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812552"
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
