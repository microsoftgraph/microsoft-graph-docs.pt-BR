---
title: Tipo de recurso timeOffReason
description: Um motivo válido para fazer o tempo de folga na agenda.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 82b94ac3f49533372a1e67d86bdf38e07b975ece
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333950"
---
# <a name="timeoffreason-resource-type"></a>Tipo de recurso timeOffReason

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Crie um novo **timeOffReason**.|
|[Lista](../api/schedule-list-timeoffreasons.md) | [Coleção timeOffReason](timeoffreason.md) | Obter a lista **de timeOffReason** em um cronograma.|
|[Get](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Obter um **timeOffReason** por ID.|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Substitua um **timeOffReason**.|
|[Delete](../api/timeoffreason-delete.md) | Nenhum | Marque um **timeOffReason** como inativo.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |ID do **timeOffReason**.|
| displayName               | `string`                  | O nome do **timeOffReason**. Obrigatório. |
| iconType | `timeOffReasonIconType`   | Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny. Obrigatório. |
| isActive          |`Boolean`      | Indica se o **timeOffReason** pode ser usado ao criar novas entidades ou atualizar as existentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora no **qualOffReason** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`         |O carimbo de data/hora no **qualOffReason** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade que foi atualizada pela última **vez,OffReason**.|

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


