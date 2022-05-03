---
title: tipo de recurso de operação
description: O status de uma operação de execução longa.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: teamwork
author: billbliss
ms.openlocfilehash: c1f07f81754b1cf0373917bbb59953fd1342d627
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176516"
---
# <a name="operation-resource-type"></a>tipo de recurso de operação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O status de uma operação de execução longa.

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo            | Descrição                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | A hora de início da operação.                                                |
| id                 | Cadeia de caracteres          | A ID da operação. Somente leitura. Servidor gerado.                                  |
| lastActionDateTime | DateTimeOffset  | A hora da última ação da operação.                                   |
| status             | String          | Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


