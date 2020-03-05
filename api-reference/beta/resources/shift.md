---
title: tipo de recurso Shift
description: Um turno é uma unidade de trabalho agendado no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 16cce4d0c2ad6526154acd5895f5a24f76a7025d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520636"
---
# <a name="shift-resource-type"></a>tipo de recurso Shift

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade de trabalho agendado em um [cronograma](schedule.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar turno](../api/schedule-post-shifts.md) | [desloca](shift.md) | Criar uma página `shift`.|
|[Listar turnos](../api/schedule-list-shifts.md) | coleção [Shift](shift.md) | Obtenha a lista desse `shifts` cronograma.|
|[Obter turno](../api/shift-get.md) | [desloca](shift.md) | Obter um `shift` por ID.|
|[Substituir Shift](../api/shift-put.md) | [desloca](shift.md) | Substituir um `shift`.|
|[Excluir Shift](../api/shift-delete.md) | Nenhum | Excluir uma `shift` do agendamento.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `shift`.|
| userId            |`string`      |ID do usuário atribuído ao `shift`. Obrigatório. |
| schedulingGroupId         |`string`      |ID do grupo de agendamento do `shift` qual o faz parte. Obrigatório. |
| sharedShift   |[shiftItem](shiftitem.md)  |A versão compartilhada desse `shift` é visível por funcionários e gerentes. Obrigatório. |
| draftShift        |[shiftItem](shiftitem.md)        |A versão de rascunho desse `shift` documento que é visível por gerentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/ `shift` hora em que foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/ `shift` hora em que foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
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
