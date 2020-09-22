---
title: tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bc104f3a9c19c38ef569d08d24da83d0e07d75f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091898"
---
#  <a name="averagecomparativescore-resource-type"></a>tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por tamanho da indústria vertical, média por tamanho de estação da empresa e assim por diante) e categoria de controle (identidade, dados, dispositivo, aplicativos, infraestrutura).

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|base|Cadeia de caracteres|Tipo de escopo. Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
|averageScore|Duplo|Pontuação média dentro da base especificada.|

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
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

