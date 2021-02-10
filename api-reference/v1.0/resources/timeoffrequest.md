---
title: Tipo de recurso timeOffRequest
description: Representa um tipo de solicitação de turno a ser timeOff.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e234873110f50ed66decaa04b5462a9ff6fcf9a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154198"
---
# <a name="timeoffrequest-resource-type"></a>Tipo de recurso timeOffRequest

Namespace: microsoft.graph

Representa um tipo de solicitação de turno para [tomar timeOff](../resources/timeoff.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/timeoffrequest-get.md) | [timeOffRequest](timeoffrequest.md) | Leia as propriedades e os relacionamentos de um **objeto timeOffRequest.** |
| [Lista](../api/timeoffrequest-list.md) | [Coleção timeOffRequest](timeoffrequest.md) | Obter a lista de **objetos timeOffRequest** nesta agenda.|
| [Delete](../api/timeoffrequest-delete.md) | Nenhum | **Exclua um objeto timeOffRequest.** |
| [Aprovar](../api/timeoffrequest-approve.md)|Nenhum|Aprovar uma solicitação de folga.|
| [Recusar](../api/timeoffrequest-decline.md)|Nenhum|Recusar uma solicitação de folga.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|startDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|timeOffReasonId|Cadeia de caracteres|O motivo da folga.|

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

