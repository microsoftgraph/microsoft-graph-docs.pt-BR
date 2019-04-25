---
title: tipo de recurso plannerAssignment
description: O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto plannerAssignments.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541357"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="0ecc3-104">tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="0ecc3-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ecc3-105">O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="0ecc3-106">Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="0ecc3-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="0ecc3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ecc3-107">Properties</span></span>
| <span data-ttu-id="0ecc3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ecc3-108">Property</span></span>     | <span data-ttu-id="0ecc3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ecc3-109">Type</span></span>   |<span data-ttu-id="0ecc3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ecc3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ecc3-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="0ecc3-111">assignedBy</span></span>|[<span data-ttu-id="0ecc3-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="0ecc3-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="0ecc3-113">A identidade do usuário que realizou a atribuição da tarefa, ou seja, o destinatário.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="0ecc3-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ecc3-114">assignedDateTime</span></span>|<span data-ttu-id="0ecc3-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ecc3-115">DateTimeOffset</span></span>|<span data-ttu-id="0ecc3-116">O horário em que a tarefa foi atribuída.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-116">The time at which the task was assigned.</span></span> <span data-ttu-id="0ecc3-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ecc3-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0ecc3-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0ecc3-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="0ecc3-119">orderHint</span></span>|<span data-ttu-id="0ecc3-120">String</span><span class="sxs-lookup"><span data-stu-id="0ecc3-120">String</span></span>|<span data-ttu-id="0ecc3-121">Dica usada para ordenar destinatários em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="0ecc3-122">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="0ecc3-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ecc3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ecc3-123">JSON representation</span></span>
<span data-ttu-id="0ecc3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ecc3-124">Here is a JSON representation of the resource.</span></span>

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
