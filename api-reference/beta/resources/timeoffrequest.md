---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno para o tempo limite.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 31d855f21164f933fe27acc824759cee08e16c16
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786065"
---
# <a name="timeoffrequest-resource-type"></a>Tipo de recurso timeOffRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de solicitação de turno para [fazer timeOff](../resources/timeoff.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/timeoffrequest-list.md) | [Coleção timeOffRequest](timeoffrequest.md) | Obter a lista de **objetos timeOffRequest** nesta agenda.|
| [Get](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | Leia as propriedades e as relações de um **objeto timeOffRequest.** |
| [Delete](../api/timeoffrequest-delete.md) | Nenhuma | **Exclua um objeto timeOffRequest.** |
| [Aprovar](../api/timeoffrequest-approve.md)|Nenhuma|Aprovar uma solicitação de tempo de folga.|
| [Declínio](../api/timeoffrequest-decline.md)|Nenhuma|Recusar uma solicitação de tempo de folga.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|timeOffReasonId|String|O motivo da folga.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest"
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


