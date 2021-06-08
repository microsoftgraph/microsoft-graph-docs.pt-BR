---
title: tipo de recurso do cartão de tempo
description: Uma entrada de cartão de ponto na agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786370"
---
# <a name="timecard-resource-type"></a>tipo de recurso do cartão de tempo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entrada de cartão de ponto na agenda.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List](../api/timecard-list.md) | [coleção timeCard](timecard.md) | Obter a lista de **objetos de cartão de** ponto nesta agenda.|
|[Create](../api/timecard-post.md) | [timeCard](timecard.md) | Crie um novo **objeto de cartão de** ponto.|
|[Get](../api/timecard-get.md) | [timeCard](timecard.md) | Obter um **objeto de cartão** de ponto por ID.|
|[Replace](../api/timecard-replace.md) | Nenhuma | Substitua um **objeto de cartão de** ponto.|
|[Delete](../api/timecard-delete.md) | Nenhuma | **Exclua um objeto de** cartão de ponto da agenda.|
|[clockIn](../api/timecard-clockin.md) | [timeCard](timecard.md) | Entre para iniciar um **cartão de ponto**.|
|[clockOut](../api/timecard-clockout.md) | Nenhuma | Clock out to end a open **timecard**.|
|[startBreak](../api/timecard-startbreak.md) | Nenhuma | Inicie um **timeCardBreak** em um cartão **de ponto específico.**|
|[endBreak](../api/timecard-endbreak.md) | Nenhuma | Termine o tempo **de aberturaCardBreak** em um **cartão de ponto específico.**|
|[confirmTimeCard](../api/timecard-confirm.md) | Nenhuma | Confirme **um registro de cartão de** ponto.|

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo           |Descrição                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| id                    |`string`  |ID do **timeCard**.|
| userId                    |`string` |ID do usuário à qual o **cartão de** usuário pertence. |
| estado                 |`timeCardState`  | O estado atual do **timeCard durante** seu ciclo de vida. Os valores possíveis são: `clockedIn` `onBreak` , , , `clockedOut` `unknownFutureValue` .|
| clockInEvent       |[timeCardEvent](../resources/timecardevent.md)    | O evento de clock-in do **timeCard**. |
| clockOutEvent                 |[timeCardEvent](../resources/timecardevent.md)  |O evento de saída do **timeCard**. |
| notes                 | [itemBody](itembody.md)  |Observações sobre **o timeCard**. |
| quebras    |[Coleção timeCardBreak](timecardbreak.md)  |A lista de quebras associada ao **timeCard**.|
| originalEntry| [timeCardEntry](../resources/timecardentry.md) | O **timeCardEntry** original do **timeCard**, antes das edições do usuário. |
| confirmedBy |`confirmedBy`    | Indique se essa **entrada timeCard** está confirmada. Os valores possíveis são `none`, `user`, `manager`, `unknownFutureValue`.|
|createdDateTime|`Edm.dateTimeOffset`| O timestamp no qual o **timeCard** foi criado. |
|createdBy|`IdentitySet`| Identidade da pessoa que criou a entidade. |
|lastModifiedDateTime|`dateTimeOffset`| O timestamp no qual **o timeCard** foi modificado pela última vez.|
|lastModifiedBy| `IdentitySet`| Identidade da pessoa que modificou a entidade pela última vez.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
