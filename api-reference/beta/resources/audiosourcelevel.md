---
title: tipo de recurso de audioSourceLevel
description: Configuração de nível de outras fontes.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: adf3c4805271d0a8d02d25fc8e7ecb547db10215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880637"
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
