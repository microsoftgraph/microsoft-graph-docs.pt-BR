---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 49d877859202ca9d8dc5c7b414368a63d2fcf8ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058093"
---
# <a name="shift-resource-type"></a>tipo de recurso Shift

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade de trabalho agendado em um [cronograma](schedule.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar turno](../api/schedule-post-shifts.md) | [shift](shift.md) | Criar uma página `shift`.|
|[Listar turnos](../api/schedule-list-shifts.md) | coleção [Shift](shift.md) | Obtenha a lista desse `shifts` cronograma.|
|[Obter turno](../api/shift-get.md) | [shift](shift.md) | Obter um `shift` por ID.|
|[Substituir Shift](../api/shift-put.md) | [shift](shift.md) | Substituir um `shift`.|
|[Excluir Shift](../api/shift-delete.md) | Nenhum | Excluir uma `shift` do agendamento.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `shift`.|
| userId            |`string`      |ID do usuário atribuído ao `shift` . Obrigatório. |
| schedulingGroupId         |`string`      |ID do grupo de agendamento do qual o `shift` faz parte. Obrigatório. |
| sharedShift   |[shiftItem](shiftitem.md)  |A versão compartilhada desse `shift` é visível por funcionários e gerentes. Obrigatório. |
| draftShift        |[shiftItem](shiftitem.md)        |A versão de rascunho desse documento `shift` que é visível por gerentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora em que `shift` foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora em que `shift` foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade da última atualização `shift`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


