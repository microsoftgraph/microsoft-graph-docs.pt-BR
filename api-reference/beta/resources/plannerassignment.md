---
title: Tipo de recurso plannerAssignment
description: O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto plannerAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522501"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="fa322-104">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="fa322-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa322-p102">O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="fa322-p102">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="fa322-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa322-107">Properties</span></span>
| <span data-ttu-id="fa322-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa322-108">Property</span></span>     | <span data-ttu-id="fa322-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa322-109">Type</span></span>   |<span data-ttu-id="fa322-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa322-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa322-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="fa322-111">assignedBy</span></span>|[<span data-ttu-id="fa322-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="fa322-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="fa322-113">A identidade do usuário que executou a atribuição da tarefa, ou seja, a atribuidor.</span><span class="sxs-lookup"><span data-stu-id="fa322-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="fa322-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa322-114">assignedDateTime</span></span>|<span data-ttu-id="fa322-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa322-115">DateTimeOffset</span></span>|<span data-ttu-id="fa322-p103">A hora que a tarefa foi atribuída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fa322-p103">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fa322-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="fa322-119">orderHint</span></span>|<span data-ttu-id="fa322-120">String</span><span class="sxs-lookup"><span data-stu-id="fa322-120">String</span></span>|<span data-ttu-id="fa322-p104">Dica usada para ordenar destinatários em uma tarefa. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="fa322-p104">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa322-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa322-123">JSON representation</span></span>
<span data-ttu-id="fa322-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa322-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
