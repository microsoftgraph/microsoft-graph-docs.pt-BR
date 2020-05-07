---
title: tipo de recurso Shift
description: Representa uma unidade de trabalho agendado no cronograma.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e38b8a000829ead91bdee28779a0f6988dd936ef
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154301"
---
# <a name="shift-resource-type"></a>tipo de recurso Shift

Namespace: microsoft.graph

Representa uma unidade de trabalho agendado em uma [agenda](schedule.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar turnos](../api/schedule-list-shifts.md) | coleção [Shift](shift.md) | Obtenha a lista de **turnos** neste cronograma.|
|[Criar turno](../api/schedule-post-shifts.md) | [desloca](shift.md) | Criar um novo **turno**.|
|[Obter turno](../api/shift-get.md) | [desloca](shift.md) | Obter um **turno** por ID.|
|[Substituir Shift](../api/shift-put.md) | [desloca](shift.md) | Substitua um **Shift**.|
|[Excluir Shift](../api/shift-delete.md) | Nenhum | Excluir uma **mudança** do cronograma.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |ID do **turno**.|
| userId            |`string`      |ID do usuário atribuído ao **turno**. Obrigatório. |
| schedulingGroupId         |`string`      |ID do grupo de agendamento do qual o **turno** faz parte. Obrigatório. |
| sharedShift   |[shiftItem](shiftitem.md)  |A versão compartilhada dessa **mudança** que é visível por funcionários e gerentes. Obrigatório. |
| draftShift        |[shiftItem](shiftitem.md)        |A versão de rascunho desse **turno** que é visível por gerentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora em que essa **mudança** foi criada pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`        |O carimbo de data/hora em que este **turno** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade que atualizou este **turno**pela última vez.|

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
