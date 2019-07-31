---
title: tipo de recurso timeOffReason
description: Uma razão válida para ser demorada no cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 62943670a0c87d34fd849e988ef5bf827aa6d72a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964274"
---
# <a name="timeoffreason-resource-type"></a>tipo de recurso timeOffReason

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma razão válida para uma instância do [timeOff](timeoff.md) em um [cronograma](schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar timeOffReason](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | Criar uma página `timeOffReason`.|
|[Listar timeOffReason](../api/schedule-list-timeoffreasons.md) | coleção [timeOffReason](timeoffreason.md) | Obter uma lista dos `timeOffReasons` em um cronograma.|
|[Obter timeOffReason](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | Obter um `timeOffReason` por ID.|
|[Substituir timeOffReason](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | Substituir um `timeOffReason`.|
|[Excluir timeOffReason](../api/timeoffreason-delete.md) | Nenhum | Marcar `timeOffReason` como inativa.|

## <a name="properties"></a>Propriedades
|Nome          |Tipo           |Descrição                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |A ID da tarefa `timeOffReason`.|
| Nome para exibição               | `string`                  | O nome do `timeOffReason`. Obrigatório. |
| icontype | `timeOffReasonIconType`   | Tipos de ícone suportados: nenhum; automóvel dos com plano firstAid; Doutor Não funciona; medição juryDuty; Globe copo telefone Weather abrangência piggyBank; cachorro torta trafficCone; pessoal ensolarado. Obrigatório. |
| isActive          |`Boolean`      | Indica se o `timeOffReason` pode ser usada na criação de novas entidades ou atualizar as existentes. Obrigatório. |
| createdDateTime       |`DateTimeOffset`        |O carimbo de data/hora `timeOffReason` em que foi criado pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| lastModifiedDateTime      |`DateTimeOffset`         |O carimbo de data/hora `timeOffReason` em que foi atualizado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
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
