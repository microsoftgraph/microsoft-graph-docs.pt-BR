---
title: " Tipo de recurso averageComparativeScore"
description: Esse recurso contém várias pontuações diferentes com base em diferentes escopos (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4c563d8754ba5afb1c4fe89d237f978d886f9eab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064606"
---
#  <a name="averagecomparativescore-resource-type"></a>Tipo de recurso averageComparativeScore

Namespace: microsoft.graph

Esse recurso contém várias pontuações diferentes com base em diferentes escopos (por exemplo, média por setor vertical, média por tamanho de assento da empresa e assim por diante) e categoria de controle (Identidade, Dados, Dispositivo, Aplicativos, Infraestrutura).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|   base   |   String  |   Tipo de escopo (Por AllTenants, TotalSeats, IndustryTypes).  |
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


