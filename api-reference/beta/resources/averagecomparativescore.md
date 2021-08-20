---
title: " Tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em diferentes escopos (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7a09d3b2c6457063457eee4a4bfbe3d1f88823f8864f66ac4a1ea690e33c77e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210145"
---
#  <a name="averagecomparativescore-resource-type"></a>Tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Esse recurso contém várias pontuações diferentes com base em diferentes escopos (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   Cadeia de caracteres  |   Tipo de escopo (Por AllTenants, TotalSeats, IndustryTypes).  |
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


