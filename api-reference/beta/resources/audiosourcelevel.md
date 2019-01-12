---
title: tipo de recurso de audioSourceLevel
description: Configuração de nível de outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79ad56c11e8b277a1354ffc3a6292a0434466c8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947649"
---
# <a name="audiosourcelevel-resource-type"></a>tipo de recurso de audioSourceLevel

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Configuração de nível de outras fontes.

## <a name="properties"></a>Propriedades

| Propriedade               | Tipo    | Descrição                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Booliano | Habilita a essa fonte para jantar de outras fontes enquanto estão ativos. Se definido como true, desviando nível deve ser definido.|
| nível                  | Int64   | Desviando nível da fonte se `duckOthers` estiver definida como `true`.                                     |
| participante            | Cadeia de caracteres  | O fluxo de áudio participante do código-fonte.                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
