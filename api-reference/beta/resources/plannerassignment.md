---
title: Tipo de recurso plannerAssignment
description: O **recurso plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto plannerAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d9e608b027200566fc957b3c267e56b599d7b0cb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721163"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="6469f-104">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="6469f-104">plannerAssignment resource type</span></span>

<span data-ttu-id="6469f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6469f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6469f-106">O **recurso plannerAssignment** representa a atribuição de uma tarefa a um usuário.</span><span class="sxs-lookup"><span data-stu-id="6469f-106">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="6469f-107">Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="6469f-107">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="6469f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6469f-108">Properties</span></span>
| <span data-ttu-id="6469f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6469f-109">Property</span></span>     | <span data-ttu-id="6469f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6469f-110">Type</span></span>   |<span data-ttu-id="6469f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6469f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6469f-112">assignedBy</span><span class="sxs-lookup"><span data-stu-id="6469f-112">assignedBy</span></span>|[<span data-ttu-id="6469f-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="6469f-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="6469f-114">A identidade do usuário que realizou a atribuição da tarefa, ou seja, o atribuídor.</span><span class="sxs-lookup"><span data-stu-id="6469f-114">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="6469f-115">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6469f-115">assignedDateTime</span></span>|<span data-ttu-id="6469f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6469f-116">DateTimeOffset</span></span>|<span data-ttu-id="6469f-117">O momento em que a tarefa foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="6469f-117">The time at which the task was assigned.</span></span> <span data-ttu-id="6469f-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6469f-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6469f-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6469f-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6469f-120">orderHint</span><span class="sxs-lookup"><span data-stu-id="6469f-120">orderHint</span></span>|<span data-ttu-id="6469f-121">String</span><span class="sxs-lookup"><span data-stu-id="6469f-121">String</span></span>|<span data-ttu-id="6469f-122">Dica usada para ordenar os atribuídos em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="6469f-122">Hint used to order assignees in a task.</span></span> <span data-ttu-id="6469f-123">O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="6469f-123">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6469f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6469f-124">JSON representation</span></span>
<span data-ttu-id="6469f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6469f-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


