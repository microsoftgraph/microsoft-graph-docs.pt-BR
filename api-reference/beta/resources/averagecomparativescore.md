---
title: " tipo de recurso de averageComparativeScore"
description: Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834591"
---
#  <a name="averagecomparativescore-resource-type"></a>tipo de recurso de averageComparativeScore

Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   Cadeia de caracteres  |   Tipo de escopo (por AllTenants, TotalSeats, IndustryTypes).  |
|   Média    |   Duplo  | Pontuação média dentro de base especificada. |
|   deviceScore |   Duplo  | Pontuação média dentro de base especificada. |
|   dataScore   |   Duplo  | Pontuação média dentro de base especificada. |
|   identityScore   |   Duplo  | Pontuação média dentro de base especificada. |

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
