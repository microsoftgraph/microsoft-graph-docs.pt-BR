---
title: tipo de recurso cancelMediaProcessingOperation
description: Esse tipo de recurso é usado para descrever o formato de resposta da operação de processamento de mídia cancelada.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b7cecdfbbb6ced93149740de89a18081a04cffa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078935"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>Tipo de recurso CancelMediaProcessingOperation

Namespace: microsoft.graph

Descreve o formato de resposta da operação de processamento de mídia cancelada.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                        | Descrição                                                                     |
| :------------ | :-------------------------- | :------------------------------------------------------------------------------ |
| all           | Boolean                     | Indica se todas as operações ou atuais são paradas.                            |
| clientContext | String                      | O contexto do cliente.                                                             |
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

