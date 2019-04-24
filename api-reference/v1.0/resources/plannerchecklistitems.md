---
title: tipo de recurso plannerChecklistItems
description: O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa. É um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto checklistItem.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 17c1d8c0529e0d85ebc784d25c2dc284f1775c0f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462281"
---
# <a name="plannerchecklistitems-resource-type"></a><span data-ttu-id="521d6-106">tipo de recurso plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="521d6-106">plannerChecklistItems resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="521d6-107">O recurso **plannerChecklistItemCollection** representa a coleção de itens de lista de verificação em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="521d6-107">The **plannerChecklistItemCollection** resource represents the collection of checklist items on a task.</span></span> <span data-ttu-id="521d6-108">É um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="521d6-108">It is an Open Type.</span></span> <span data-ttu-id="521d6-109">Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="521d6-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="521d6-110">O valor no par propriedade-valor é o objeto [checklistItem](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="521d6-110">The value in the property-value pair is the [checklistItem](plannerchecklistitem.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="521d6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="521d6-111">Properties</span></span>
<span data-ttu-id="521d6-112">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="521d6-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="521d6-113">Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser objetos [checklistItem](plannerchecklistitem.md) .</span><span class="sxs-lookup"><span data-stu-id="521d6-113">In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects.</span></span> <span data-ttu-id="521d6-114">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="521d6-114">Example is shown below.</span></span> <span data-ttu-id="521d6-115">Para remover um item da lista de verificação, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="521d6-115">To remove an item in the checklist, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="521d6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="521d6-116">JSON representation</span></span>

<span data-ttu-id="521d6-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="521d6-117">Here is a JSON representation of the resource</span></span>

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
<span data-ttu-id="521d6-118">Como</span><span class="sxs-lookup"><span data-stu-id="521d6-118">// Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitems.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
