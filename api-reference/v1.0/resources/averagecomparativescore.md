---
title: Tipo de recurso averageComparativeScore
description: Contém várias pontuações diferentes com base em escopos diferentes.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 88444bfab00622a6ac8cc89a3af287650ad1af7e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899971"
---
#  <a name="averagecomparativescore-resource-type"></a>Tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|Base|Cadeia de Caracteres|Tipo de escopo. Os valores possíveis são: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
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

