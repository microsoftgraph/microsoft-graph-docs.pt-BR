---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 47937d059f9a624ca5b9c58333275081d5a68400
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865665"
---
# <a name="commsoperation-resource-type"></a>tipo de recurso commsOperation

Representa o status de determinadas operações de longa duração.

Esse recurso pode ser retornado como a resposta a uma ação ou como o conteúdo de um [commsNotification](commsNotification.md).  

Quando ele é retornado como uma resposta a uma ação, o status indica se haverá notificações subsequentes. Se, por exemplo, uma operação com status `completed` ou `failed` for retornada, não haverá nenhuma operação subsequente por meio do canal de notificação. 

Se uma `null` operação ou uma operação com o status `notStarted` ou `running` for retornada, as atualizações subsequentes serão fornecidas pelo canal de notificação.

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                        | Descrição                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | Cadeia de caracteres de contexto de cliente exclusivo. O limite máximo é de 256 caracteres.                           |
| id                 | Cadeia de caracteres                      | A ID da operação. Somente leitura.                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | As informações de resultado. Somente leitura.                                              |
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
