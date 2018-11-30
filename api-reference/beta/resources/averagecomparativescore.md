---
title: " tipo de recurso de averageComparativeScore"
description: Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034440"
---
#  <a name="averagecomparativescore-resource-type"></a>tipo de recurso de averageComparativeScore

Este recurso contém vários pontuações diferentes com base em por categoria de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura) e escopos diferentes (por exemplo, média pelo setor vertical, média pelo tamanho da estação de empresa e assim por diante).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   String  |   Tipo de escopo (por AllTenants, TotalSeats, IndustryTypes).  |
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
