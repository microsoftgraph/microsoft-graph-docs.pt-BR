---
title: Tipo de recurso timeOffReason
description: Um motivo válido para fazer o tempo de folga na agenda.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b449f2cb4dcfcd73208d58f8e1e969b9a701e54b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720183"
---
# <a name="timeoffreason-resource-type"></a>Tipo de recurso timeOffReason

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Crie um novo **timeOffReason**.|
|[List](../api/schedule-list-timeoffreasons.md) | [Coleção timeOffReason](timeoffreason.md) | Obter a lista **de timeOffReason** em um cronograma.|
|[Get](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Obter um **timeOffReason** por ID.|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Substitua um **timeOffReason**.|
|[Delete](../api/timeoffreason-delete.md) | Nenhum(a) | Marque um **timeOffReason** como inativo.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `timeOffReason`.|
| Nome para exibição               | `string`                  | O nome do `timeOffReason` . Obrigatório. |
| iconType | `timeOffReasonIconType`   | Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny. Obrigatório. |
| isActive          |`Boolean`      | Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora no `timeOffReason` qual isso foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`         |O carimbo de data/hora no qual `timeOffReason` foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade da última atualização `timeOffReason`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


