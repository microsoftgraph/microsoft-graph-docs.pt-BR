---
title: tipo de recurso timeOff
description: Uma unidade de não trabalho no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 060d155b713b46c36dc5c3c4eed433142822857d
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537027"
---
# <a name="timeoff-resource-type"></a>tipo de recurso timeOff

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade de não trabalho no cronograma.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar timeOff](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | Criar um novo `timeOff` objeto.|
|[Listar timeoffss](../api/schedule-list-timesoff.md) | coleção [timeOff](timeoff.md) | Obtenha a lista de `timeOff` objetos nesse cronograma.|
|[Obter timeOff](../api/timeoff-get.md) | [timeOff](timeoff.md) | Obter um `timeOff` por ID.|
|[Substituir timeOff](../api/timeoff-put.md) | [timeOff](timeoff.md) | Substituir um `timeOff`.|
|[Excluir timeOff](../api/timeoff-delete.md) | Nenhum | Excluir uma `timeOff` do agendamento.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `timeOff`.|
| userId            |`string`      |ID do usuário atribuído ao `timeOff`. Obrigatório.|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |A versão compartilhada desse `timeOff` é visível por funcionários e gerentes. Obrigatório.|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |A versão de rascunho desse `timeOff` documento que é visível por gerentes. Obrigatório.|
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora `timeOff` em que foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora `timeOff` em que foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade da última atualização `timeOff`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
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
  "suppressions": []
}
-->
