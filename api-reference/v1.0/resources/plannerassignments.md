# <a name="plannerassignments-resource-type"></a><span data-ttu-id="82d2a-101">Tipo de recurso plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="82d2a-101">plannerAssignments resource type</span></span>

<span data-ttu-id="82d2a-p101">O recurso **plannerAssignment** representa as atribuições de um recurso [plannerTask](plannertask.md). Este é um Tipo Aberto. Cada nome de propriedade nesse tipo representa a ID do objeto de um usuário à qual uma tarefa é atribuída. Os usuários podem ser atribuídos a tarefas com a criação de novas propriedades nomeadas com sua ID, com um objeto [plannerassignment](plannerassignment.md) com a propriedade orderHint preenchida como o valor. Os destinatários podem ter a atribuição cancelada a partir da tarefa se a propriedade nomeada com a ID for configurada como nula.</span><span class="sxs-lookup"><span data-stu-id="82d2a-p101">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="82d2a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82d2a-107">Properties</span></span>
<span data-ttu-id="82d2a-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. No entanto, nesse caso, o cliente deve fornecer IDs do usuário atribuídas como nomes de propriedades. A propriedade deve ser definida com um objeto **plannerAssignment** para criar ou modificar os destinatários e como nula para removê-los.</span><span class="sxs-lookup"><span data-stu-id="82d2a-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="82d2a-111">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="82d2a-111">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
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
<span data-ttu-id="82d2a-p103">Este exemplo remove usuário com a ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 da lista de destinatários da tarefa ao alterar a ordem dos destinatário com o usuário ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. Se a tarefa já não estiver atribuída ao usuário com a ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, a tarefa será atribuída a esse usuário se as atribuições forem atualizadas com esse valor.</span><span class="sxs-lookup"><span data-stu-id="82d2a-p103">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->