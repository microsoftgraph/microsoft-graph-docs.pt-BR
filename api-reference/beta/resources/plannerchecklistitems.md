---
title: tipo de recurso plannerChecklistItems
description: O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto checklistItem.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5816be4175e719077836ad103a524acce86c0a1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521759"
---
# <a name="plannerchecklistitems-resource-type"></a>tipo de recurso plannerChecklistItems

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um tipo aberto. Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) . O valor no par propriedade-valor é o objeto [checklistItem](plannerchecklistitem.md) .


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser objetos [checklistItem](plannerchecklistitem.md) . O exemplo é mostrado abaixo. Para remover um item da lista de verificação, defina o valor da propriedade como `null`.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
Como

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
