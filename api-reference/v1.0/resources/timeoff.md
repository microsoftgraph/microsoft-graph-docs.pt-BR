---
title: Tipo de recurso timeOff
description: Uma unidade que não funciona na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 9390ec6e148bde2a5edab6b9984561a878d2d0d88e25078d4ecbbd7b50f2a63f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196477"
---
# <a name="timeoff-resource-type"></a>Tipo de recurso timeOff

Namespace: microsoft.graph

Uma unidade que não funciona em um cronograma.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/schedule-list-timesoff.md) | [Coleção timeOff](timeoff.md) | Obter a lista de **objetos timeOff** nesta agenda.|
|[Criar](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | Crie um novo **objeto timeOff.**|
|[Obter](../api/timeoff-get.md) | [timeOff](timeoff.md) | Obter um **objeto timeOff** por ID.|
|[Replace](../api/timeoff-put.md) | [timeOff](timeoff.md) | Substitua um **objeto timeOff.**|
|[Delete](../api/timeoff-delete.md) | None | **Exclua um objeto timeOff** da agenda.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID do **timeOff**.|
| userId            |`string`      |ID do usuário atribuído ao **timeOff**. Obrigatório.|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |A versão compartilhada deste **timeOff** que pode ser visualizada por funcionários e gerentes. Obrigatório.|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |A versão de rascunho deste **timeOff** que pode ser visualizada pelos gerentes. Obrigatório.|
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora no **qual este timeOff** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora no **qual o timeOff** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade que foi atualizada pela última vez **desta vezOff**. |

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

