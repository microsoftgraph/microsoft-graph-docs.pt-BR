---
title: tipo de recurso shift
description: Um turno é uma unidade de trabalho agendada na agenda.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52b170fef5a283cfaa31199d78bd943212539434
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334440"
---
# <a name="shift-resource-type"></a>tipo de recurso shift

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade de trabalho agendada em um [cronograma](schedule.md). 

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar turno](../api/schedule-post-shifts.md) | [shift](shift.md) | Criar uma página `shift`.|
|[Listar turnos](../api/schedule-list-shifts.md) | [coleção shift](shift.md) | Obter a lista de `shifts` nesta agenda.|
|[Obter turno](../api/shift-get.md) | [shift](shift.md) | Obter um `shift` por ID.|
|[Substituir turno](../api/shift-put.md) | [shift](shift.md) | Substituir um `shift`.|
|[Excluir turno](../api/shift-delete.md) | Nenhum(a) | Exclua um `shift` da agenda.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `shift`.|
| userId            |`string`      |ID do usuário atribuído ao `shift`. Obrigatório. |
| schedulingGroupId         |`string`      |ID do grupo de agendamento `shift` do que faz parte. Obrigatório. |
| sharedShift   |[shiftItem](shiftitem.md)  |A versão compartilhada disso que `shift` pode ser visualizada por funcionários e gerentes. Obrigatório. |
| draftShift        |[shiftItem](shiftitem.md)        |A versão de rascunho disso que `shift` pode ser visualizada pelos gerentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O timestamp no qual isso `shift` foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |O data/hora no qual isso foi `shift` atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
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


