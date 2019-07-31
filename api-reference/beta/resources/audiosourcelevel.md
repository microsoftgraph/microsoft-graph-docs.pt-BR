---
title: tipo de recurso audioSourceLevel
description: Configuração de nível para outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa3a06d319eea0e3af5c016a9ef799591f76fabb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013210"
---
# <a name="audiosourcelevel-resource-type"></a>tipo de recurso audioSourceLevel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configuração de nível para outras fontes.

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo    | Descrição                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Booliano | Permite que essa fonte para o pato de outras fontes enquanto ativa. Se for definido como true, o nível de pato precisará ser definido.|
| antes                  | Int64   | O nível de pato da origem se `duckOthers` estiver definido como `true`.                                     |
| participante            | String  | O fluxo de áudio do participante de origem.                                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
