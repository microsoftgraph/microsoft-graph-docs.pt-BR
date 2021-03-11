---
title: Tipo de recurso securityActionState
description: Representa o histórico de alterações de estado securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6a2fecbc05c9987ee8daec8fa017d728a2d03ed3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722087"
---
# <a name="securityactionstate-resource-type"></a>Tipo de recurso securityActionState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o histórico de alterações de estado securityAction.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appId|Cadeia de caracteres|A ID do Aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) à ação. O deve ser extraído do token de auth e não inserido `appId` manualmente pelo aplicativo de chamada.|
|status|Cadeia de caracteres| Status da securityAction nesta atualização. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|updatedDateTime|DateTimeOffset| Timestamp quando actionState foi atualizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|user|Cadeia de caracteres|O nome principal do usuário do usuário que enviou uma atualização (PATCH) à ação. O deve ser extraído do token de auth e não inserido `user` manualmente pelo aplicativo de chamada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


