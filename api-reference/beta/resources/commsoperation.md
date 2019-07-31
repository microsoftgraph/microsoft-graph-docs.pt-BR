---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012895"
---
# <a name="commsoperation-resource-type"></a>tipo de recurso commsOperation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O status de determinadas operações de longa duração.

## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                        | Descrição                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | O contexto do cliente.                                                             |
| createdDateTime    | DateTimeOffset              | A hora de início da operação.                                                |
| id                 | Cadeia de caracteres                      | A ID da operação. Somente leitura. Servidor gerado.                                  |
| lastActionDateTime | DateTimeOffset              | A hora da última ação da operação.                                   |
| resultInfo         | [resultInfo](resultinfo.md) | As informações de resultado. Somente leitura. Servidor gerado.                            |
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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
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
