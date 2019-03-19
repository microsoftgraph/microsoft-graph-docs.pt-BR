---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676986"
---
# <a name="timeoff-resource-type"></a>tipo de recurso timeOff

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade de não trabalho no cronograma.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar timeOff](../api/schedule-post-timesoff.md) | [timeOff](timeOff.md) | Criar um novo `timeOff` objeto.|
|[Listar timeOffss](../api/schedule-list-timesoff.md) | coleção [timeOff](timeOff.md) | Obtenha a lista de `timeOff` objetos nesse cronograma.|
|[Obter timeOff](../api/timeoff-get.md) | [timeOff](timeOff.md) | Obter a `timeOff` por ID.|
|[Substituir timeOff](../api/timeoff-put.md) | [timeOff](timeOff.md) | Substitua um `timeOff`.|
|[Excluir timeOff](../api/timeoff-delete.md) | Nenhum | Excluir uma `timeOff` do agendamento.|

## <a name="properties"></a>Propriedades
|Name          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID do `timeOff`.|
| userId            |`string`      |ID do usuário atribuído ao `timeOff`. Obrigatório.|
| sharedTimeOff     |[timeOffItem](timeoffitem.md)  |A versão compartilhada desse `timeOff` é visível por funcionários e gerentes. Obrigatório.|
| draftTimeOff      |[timeOffItem](timeoffitem.md)        |A versão de rascunho desse `timeOff` documento que é visível por gerentes. Obrigatório.|
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora `timeOff` em que foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora `timeOff` em que foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '. |
| lastModifiedBy        |`microsoft.graph.identitySet`        |A identidade que foi atualizada pela `timeOff`última vez. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
