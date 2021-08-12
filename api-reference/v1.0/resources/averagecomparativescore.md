---
title: Tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2041a366fcf37ff8a850fb8d6fd41e9c3fd6002a17916d41718588674a30a3e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147018"
---
#  <a name="averagecomparativescore-resource-type"></a>Tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).

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

