---
title: " Tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: b5cf6482b76180a64e2ec468648a48113377114d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900209"
---
#  <a name="averagecomparativescore-resource-type"></a>Tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Esse recurso contém várias pontuações diferentes com base em escopos diferentes (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   Base   |   Cadeia de Caracteres  |   Tipo de escopo (Por AllTenants, TotalSeats, IndustryTypes).  |
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


