---
title: tipo de recurso de audioDuckingConfiguration
description: Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d61e4150250df25e020f45a65676d1c55c0e4c9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522459"
---
# <a name="audioduckingconfiguration-resource-type"></a>tipo de recurso de audioDuckingConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Parâmetros para desviando de outras fontes (Introdução gradual e sair de outras fontes.)

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo     | Descrição                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | O volume das fontes em % quando as fontes estão sendo ducked.             |
| rampActive    | Int64    | A quantidade de tempo (em milissegundos) que leva para fontes ducked "desaparecer". |
| rampInactive  | Int64    | A quantidade de tempo (em milissegundos) que leva para ducked fontes para "desaparecer".  |
| upperLevel    | Int64    | O volume das fontes em % quando as fontes não estão sendo ducked.         |

> **Observação:** Duração conheça não pode ser mais de 5.000 milissegundos.

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioduckingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
