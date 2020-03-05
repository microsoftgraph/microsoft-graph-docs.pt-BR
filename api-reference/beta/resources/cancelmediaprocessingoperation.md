---
title: Tipo de recurso CancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de cancelamento do processamento de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 700c63b2b620117f25df876544aeb6fb0e6d0230
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507779"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Tipo de recurso CancelMediaProcessingOperation

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o formato de resposta da operação de cancelamento do processamento de mídia.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| todos os                            | Boolean                     | Indica se todas as operações ou atuais serão interrompidas.                                                                                    |
| clientContext                  | String                      | O contexto do cliente.                                                                                                                               |
| id                             | Cadeia de caracteres                      | A ID da operação do servidor. Somente leitura.                                                                                              |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                                                                              |
| status                         | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                  |

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
