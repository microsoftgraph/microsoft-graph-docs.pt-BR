---
title: tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de mudança para obter timeoff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73fa72d403bd20e6a966b01a0529d09689e5ed66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519712"
---
# <a name="timeoffrequest-resource-type"></a>tipo de recurso timeOffRequest

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de solicitação de mudança para obter [timeoff](../resources/timeoff.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | Leia as propriedades e os relacionamentos de um objeto **timeOffRequest** . |
| [Update](../api/timeoffrequest-update.md) | [timeOffRequest](timeoffrequest.md) | Atualizar um objeto **timeOffRequest** . |
| [Delete](../api/timeoffrequest-delete.md) | None | Excluir um objeto **timeOffRequest** . |
|[Aprovar](../api/timeoffrequest-approve.md)|Nenhum|Aprovar uma solicitação de tempo limite.|
|[Aceito](../api/timeoffrequest-decline.md)|Nenhum|Recusar uma solicitação de tempo limite.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|timeOffReasonId|String|O motivo da folga.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
