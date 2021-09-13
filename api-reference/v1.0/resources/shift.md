---
title: tipo de recurso shift
description: Representa uma unidade de trabalho agendada na agenda.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3b00e93f4622b91e7abe92a68007e870b5ab432e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032220"
---
# <a name="shift-resource-type"></a>tipo de recurso shift

Namespace: microsoft.graph

Representa uma unidade de trabalho agendada em um [cronograma](schedule.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar turnos](../api/schedule-list-shifts.md) | [coleção shift](shift.md) | Obter a lista **de turnos** nesta agenda.|
|[Criar turno](../api/schedule-post-shifts.md) | [shift](shift.md) | Criar um novo **turno**.|
|[Obter turno](../api/shift-get.md) | [shift](shift.md) | Obter um **turno** por ID.|
|[Substituir turno](../api/shift-put.md) | [shift](shift.md) | Substitua um **turno**.|
|[Excluir turno](../api/shift-delete.md) | None | **Exclua um turno** da agenda.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID do **turno**.|
| userId            |`string`      |ID do usuário atribuído ao **turno**. Obrigatório. |
| schedulingGroupId         |`string`      |A ID do grupo de agendamento **do turno** faz parte. Obrigatório. |
| sharedShift   |[shiftItem](shiftitem.md)  |A versão compartilhada **dessa** mudança que pode ser visualizada por funcionários e gerentes. Obrigatório. |
| draftShift        |[shiftItem](shiftitem.md)        |A versão de rascunho dessa **mudança** que pode ser visualizada pelos gerentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O data/hora no qual esse **turno** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`        |O data/hora no qual esse **turno** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade que atualizou pela última vez esse **turno**.|

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

