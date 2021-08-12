---
title: Tipo de recurso plannerChecklistItems
description: O **recurso plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um Tipo Aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par de valores de propriedade é o objeto checklistItem.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f465adf89e9cb344013e30edccf03513f8fb96065e676ffb78d7cb8fa13f14ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178070"
---
# <a name="plannerchecklistitems-resource-type"></a>Tipo de recurso plannerChecklistItems

Namespace: microsoft.graph

O **recurso plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um Tipo Aberto. Ele faz parte do objeto [de detalhes da](plannertaskdetails.md) tarefa. O valor no par de valores de propriedade é o [objeto checklistItem.](plannerchecklistitem.md)


## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser [objetos checklistItem.](plannerchecklistitem.md) Exemplo é mostrado abaixo. Para remover um item na lista de verificação, defina o valor da propriedade como `null` .

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
Exemplo

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

