---
title: Tipo de recurso plannerAssignment
description: O recurso de **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado em plannerAssignments do tipo aberto.
localization_priority: Normal
ms.openlocfilehash: a2766653fdd7fe29c40529e77bbff2c72e8e6be7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875681"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="58560-104">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="58560-104">plannerAssignment resource type</span></span>

<span data-ttu-id="58560-p102">O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="58560-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="58560-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58560-107">Properties</span></span>
| <span data-ttu-id="58560-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58560-108">Property</span></span>     | <span data-ttu-id="58560-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="58560-109">Type</span></span>   |<span data-ttu-id="58560-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58560-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58560-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="58560-111">assignedBy</span></span>|[<span data-ttu-id="58560-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="58560-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="58560-113">A identidade do usuário que executou a atribuição da tarefa, ou seja, a atribuidor.</span><span class="sxs-lookup"><span data-stu-id="58560-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="58560-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="58560-114">assignedDateTime</span></span>|<span data-ttu-id="58560-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58560-115">DateTimeOffset</span></span>|<span data-ttu-id="58560-p103">A hora que a tarefa foi atribuída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58560-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58560-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="58560-119">orderHint</span></span>|<span data-ttu-id="58560-120">String</span><span class="sxs-lookup"><span data-stu-id="58560-120">String</span></span>|<span data-ttu-id="58560-p104">Dica usada para ordenar destinatários em uma tarefa. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="58560-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58560-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58560-123">JSON representation</span></span>
<span data-ttu-id="58560-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58560-124">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
