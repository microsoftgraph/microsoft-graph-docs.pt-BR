---
title: tipo de recurso audioDuckingConfiguration
description: Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013217"
---
# <a name="audioduckingconfiguration-resource-type"></a>tipo de recurso audioDuckingConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Parâmetros para o pato de outras fontes (phasing dentro e fora de outras fontes).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo     | Descrição                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | O volume de fontes em porcentagem quando as fontes estão sendo disparadas.             |
| rampActive    | Int64    | A quantidade de tempo (em milissegundos) que demora para que as fontes em intervalo sejam "Fade out". |
| rampInactive  | Int64    | A quantidade de tempo (em milissegundos) que demora para as fontes em um intervalo para "Fade in".  |
| upperLevel    | Int64    | O volume de fontes em porcentagem quando as fontes não estão sendo disparadas.         |

> **Observação:** A duração da rampa não pode ser maior que 5.000 milissegundos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
