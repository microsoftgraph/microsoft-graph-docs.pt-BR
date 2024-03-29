---
title: Tipo de recurso timeOffReason
description: Representa um motivo válido para o tempo de folga na agenda.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: e24c59f10e29bf3ab9e6a4948a5dc61d371d1e42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134322"
---
# <a name="timeoffreason-resource-type"></a>Tipo de recurso timeOffReason

Namespace: microsoft.graph

Representa um motivo válido para uma [instância timeOff](timeoff.md) em um [cronograma](schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/schedule-list-timeoffreasons.md) | [Coleção timeOffReason](timeoffreason.md) | Obter a lista **de timeOffReason** em um cronograma.|
|[Criar](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Crie um novo **timeOffReason**.|
|[Obter](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Obter um **timeOffReason** por ID.|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Substitua um **timeOffReason**.|
|[Delete](../api/timeoffreason-delete.md) | Nenhum(a) | Marque um **timeOffReason** como inativo.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `timeOffReason`.|
| Nome para exibição               | `string`                  | O nome do **timeOffReason**. Obrigatório. |
| iconType | `timeOffReasonIconType`   | Tipos de ícone com suporte: nenhum; car; calendar; em execução; plano; firstAid; médico; notWorking; clock; juryDuty; globe; cup; telefone; clima; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny. Obrigatório. |
| isActive          |`Boolean`      | Indica se o **timeOffReason** pode ser usado ao criar novas entidades ou atualizar as existentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora no **qualOffReason** foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime      |`DateTimeOffset`         |O carimbo de data/hora no **qualOffReason** foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| lastModifiedBy        | [identitySet](identityset.md)        |A identidade que foi atualizada pela última **vez desta vezOffReason**.|

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

