---
title: tipo de recurso securityActionState
description: Representa o histórico das alterações de estado SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ba22a03f4d4a6d03b0093ed28b8c54a7c095d037
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988860"
---
# <a name="securityactionstate-resource-type"></a>tipo de recurso securityActionState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o histórico das alterações de estado SecurityAction.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appId|String|A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) à ação. O `appId` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.|
|status|String| Status do SecurityAction nesta atualização. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|updatedDateTime|DateTimeOffset| Carimbo de data/hora em que ActionState foi atualizado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|user|String|O nome principal de usuário do usuário conectado que enviou uma atualização (PATCH) à ação. O `user` deve ser extraído do token de autenticação e não inserido manualmente pelo aplicativo de chamada.|

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


