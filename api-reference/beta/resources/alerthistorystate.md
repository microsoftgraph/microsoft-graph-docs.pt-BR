---
title: tipo de recurso alertHistoryState
description: Cada vez que um alerta é corrigido, a alteração é salva em um novo objeto de alertHistoryState e será retornada como parte do alerta modificado.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: a5dda54101264ee2ec4d01a283f96a93f1d6e5e3
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366963"
---
# <a name="alerthistorystate-resource-type"></a>tipo de recurso alertHistoryState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Cada vez que um alerta é corrigido, a alteração é salva em um novo objeto de alertHistoryState e será retornada como parte do alerta modificado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appId|String| A ID de aplicativo do aplicativo de chamada que enviou uma atualização (PATCH) para o alerta. A appId deve ser extraída do token de autenticação e não inserida manualmente pelo aplicativo de chamada. |
|assignedTo|Cadeia de caracteres| UPN de usuário ao qual o alerta foi atribuído (Observação: Alert. assignedTo só armazena o último valor/UPN). |
|comentários|String collection|Comentário inserido pelo usuário conectado.|
|comentários|String| Comentários de analista sobre o alerta nesta atualização. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|String| Valor do status do alerta (se atualizado). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.|
|updatedDateTime|DateTimeOffset| Data e hora da atualização de alerta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|user|String| O UPN do usuário conectado que atualizou o alerta (obtido do token de portador-se no modo de autenticação do usuário/delegado). |

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