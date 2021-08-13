---
title: tipo de recurso cancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de processamento de mídia cancelada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6896a7a4d08aea0c4d394bfbaef8a54bd4c789b310f0079dbbf08daac99606d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235685"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Tipo de recurso CancelMediaProcessingOperation

Namespace: microsoft.graph

Descreve o formato de resposta da operação de processamento de mídia cancelada.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                        | Descrição                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| all           | Booliano                     | Indica se todas as operações ou atuais são paradas.                            |
| clientContext | Cadeia de caracteres                      | O contexto do cliente.                                                             |
| id            | Cadeia de caracteres                      | A ID da operação do servidor. Somente leitura.                                             |
| resultInfo    | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                             |
| status        | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

