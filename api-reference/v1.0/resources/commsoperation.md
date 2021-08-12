---
title: Tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd924966c34d39ceb26e7b92077f01f085f9f6779896db439c1ae6c7a57eae9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130384"
---
# <a name="commsoperation-resource-type"></a>Tipo de recurso commsOperation

Namespace: microsoft.graph

Representa o status de determinadas operações de longa duração.

Esse recurso pode ser retornado como a resposta a uma ação ou como o conteúdo de [um commsNotification](commsNotification.md).  

Quando ele é retornado como uma resposta a uma ação, o status indica se haverá notificações subsequentes. Se, por exemplo, uma operação com status de ou for retornada, não haverá qualquer operação subsequente por meio `completed` `failed` do canal de notificação. 

Se uma operação ou uma operação com um status de ou for retornada, as atualizações `null` `notStarted` `running` subsequentes virão por meio do canal de notificação.

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                        | Descrição                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | Cadeia de caracteres                      | Cadeia de caracteres de contexto de cliente exclusiva. O limite máximo é 256 caracteres.                           |
| id                 | Cadeia de caracteres                      | A ID da operação. Somente leitura.                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | As informações de resultado. Apenas leitura.                                              |
| status             | String                      | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

