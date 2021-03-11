---
title: Tipo de recurso alertHistoryState
description: Armazena alterações feitas em alertas.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2bc1c1a58f6f7f073b6803adbee07b4b2990a0e1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722164"
---
# <a name="alerthistorystate-resource-type"></a>Tipo de recurso alertHistoryState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Armazena alterações feitas em alertas.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appId|Cadeia de caracteres| A ID do Aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) ao alerta. O appId deve ser extraído do token de auth e não inserido manualmente pelo aplicativo de chamada. |
|assignedTo|Cadeia de caracteres| UPN do usuário ao que o alerta foi atribuído (observação: alert.assignedTo armazena apenas o último valor/UPN). |
|comentários|String collection|Comentário inserido pelo usuário inserido.|
|comentários|Cadeia de caracteres| Comentários do analista sobre o alerta nesta atualização. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|Cadeia de caracteres| Valor de status do alerta (se atualizado). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.|
|updatedDateTime|DateTimeOffset| Data e hora da atualização de alerta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|user|Cadeia de caracteres| UPN do usuário que atualizou o alerta (retirado do token do portador - se no modo de auth delegado/do usuário). |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

