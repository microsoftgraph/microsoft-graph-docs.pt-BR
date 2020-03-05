---
title: tipo de recurso plannerAssignments
description: 'O recurso **plannerAssignments** representa as atribuições de um recurso plannerTask. Este tipo é um tipo aberto. Cada nome de propriedade neste tipo '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7f131b848f3cef6f6874a81d27ab565bd9165121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521794"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="a9210-105">tipo de recurso plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="a9210-105">plannerAssignments resource type</span></span>

<span data-ttu-id="a9210-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9210-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9210-107">O recurso **plannerAssignments** representa as atribuições de um recurso [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="a9210-107">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource.</span></span> <span data-ttu-id="a9210-108">Este tipo é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="a9210-108">This type is an open type.</span></span> <span data-ttu-id="a9210-109">Cada nome de propriedade desse tipo é a ID de um objeto de usuário ao qual uma tarefa é atribuída.</span><span class="sxs-lookup"><span data-stu-id="a9210-109">Each property name in this type is the ID of a user object a task is assigned to.</span></span> <span data-ttu-id="a9210-110">Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com a ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor.</span><span class="sxs-lookup"><span data-stu-id="a9210-110">The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value.</span></span> <span data-ttu-id="a9210-111">Os destinatários podem ser desatribuídos da tarefa definindo o propriedade nomeado com sua ID como nulo.</span><span class="sxs-lookup"><span data-stu-id="a9210-111">The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="a9210-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9210-112">Properties</span></span>
<span data-ttu-id="a9210-113">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a9210-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="a9210-114">Nesse caso, no entanto, o cliente deve fornecer IDs de usuário atribuídas como nomes de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a9210-114">In this case though, the client must provide assigned user's IDs as property names.</span></span> <span data-ttu-id="a9210-115">A propriedade deve ser definida como um objeto **plannerAssignment** para criar ou modificar destinatários, e como nulo para removê-los.</span><span class="sxs-lookup"><span data-stu-id="a9210-115">The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="a9210-116">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="a9210-116">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
<span data-ttu-id="a9210-117">Este exemplo remove o usuário com ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 da lista de destinatários da tarefa, enquanto altera a ordem do destinatário com a ID de usuário 4e98f8f1-BB03-4015-B8E0-19bb370949d8.</span><span class="sxs-lookup"><span data-stu-id="a9210-117">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8.</span></span> <span data-ttu-id="a9210-118">Se a tarefa ainda não estiver atribuída ao usuário com ID 4e98f8f1-BB03-4015-B8E0-19bb370949d8, a atualização das atribuições com esse valor atribuirá a tarefa a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="a9210-118">If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
