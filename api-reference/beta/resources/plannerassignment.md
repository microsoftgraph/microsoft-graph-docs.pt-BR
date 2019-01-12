---
title: Tipo de recurso plannerAssignment
description: O recurso de **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado em plannerAssignments do tipo aberto.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963959"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="e65ff-104">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="e65ff-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="e65ff-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e65ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e65ff-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e65ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e65ff-p103">O recurso **plannerAssignment** representa a atribuição de uma tarefa a um usuário. Esse tipo é usado no tipo aberto [plannerAssignments](plannerassignments.md).</span><span class="sxs-lookup"><span data-stu-id="e65ff-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="e65ff-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e65ff-109">Properties</span></span>
| <span data-ttu-id="e65ff-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e65ff-110">Property</span></span>     | <span data-ttu-id="e65ff-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e65ff-111">Type</span></span>   |<span data-ttu-id="e65ff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65ff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65ff-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="e65ff-113">assignedBy</span></span>|[<span data-ttu-id="e65ff-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="e65ff-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="e65ff-115">A identidade do usuário que executou a atribuição da tarefa, ou seja, a atribuidor.</span><span class="sxs-lookup"><span data-stu-id="e65ff-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="e65ff-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="e65ff-116">assignedDateTime</span></span>|<span data-ttu-id="e65ff-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e65ff-117">DateTimeOffset</span></span>|<span data-ttu-id="e65ff-p104">A hora que a tarefa foi atribuída. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e65ff-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e65ff-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="e65ff-121">orderHint</span></span>|<span data-ttu-id="e65ff-122">String</span><span class="sxs-lookup"><span data-stu-id="e65ff-122">String</span></span>|<span data-ttu-id="e65ff-p105">Dica usada para ordenar destinatários em uma tarefa. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="e65ff-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e65ff-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e65ff-125">JSON representation</span></span>
<span data-ttu-id="e65ff-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e65ff-126">Here is a JSON representation of the resource.</span></span>

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
