---
title: tipo de recurso plannerChecklistItems
description: O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto checklistItem.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 891e4c154faf053fd72578210b3d8602422279e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447126"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="c5f3c-106">tipo de recurso plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="c5f3c-106">plannerChecklistItems resource type</span></span>

<span data-ttu-id="c5f3c-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c5f3c-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5f3c-108">O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="c5f3c-108">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="c5f3c-109">É um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="c5f3c-109">It is an Open Type.</span></span> <span data-ttu-id="c5f3c-110">Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f3c-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="c5f3c-111">O valor no par propriedade-valor é o objeto [checklistItem](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f3c-111">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="c5f3c-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5f3c-112">Properties</span></span>
<span data-ttu-id="c5f3c-113">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5f3c-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="c5f3c-114">Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser objetos [checklistItem](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f3c-114">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="c5f3c-115">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="c5f3c-115">Example is shown below.</span></span> <span data-ttu-id="c5f3c-116">Para remover um item da lista de verificação, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="c5f3c-116">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5f3c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5f3c-117">JSON representation</span></span>

<span data-ttu-id="c5f3c-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c5f3c-118">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="c5f3c-119">Como</span><span class="sxs-lookup"><span data-stu-id="c5f3c-119">// Example</span></span>

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
