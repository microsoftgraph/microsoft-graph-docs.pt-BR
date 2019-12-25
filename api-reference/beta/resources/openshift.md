---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa87acd2065a3a56f15016bb7708e73cebe63a31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870156"
---
# <a name="openshift-resource-type"></a>tipo de recurso openShift

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/openshift-get.md) | [openShift](openshift.md) | Leia as propriedades e os relacionamentos de um objeto **openShift** . |
| [Update](../api/openshift-update.md) | [openShift](openshift.md) | Atualize um objeto **openShift** . |
| [Delete](../api/openshift-delete.md) | None | Excluir um objeto **openShift** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|Um turno aberto não publicado.|
|schedulingGroupId|String|ID do grupo de agendamento ao qual o turno aberto pertence.|
|sharedOpenShift|[openShiftItem](openshiftitem.md)|Um turno aberto publicado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
