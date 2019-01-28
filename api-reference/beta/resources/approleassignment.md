---
title: Tipo de recurso plannerAssignment
description: Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário. Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica. Você pode criar, ler, atualizar e excluir as atribuições de função.
localization_priority: Priority
ms.openlocfilehash: 6255642f47f0e1454fb64440d4938605a2de5df4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513897"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="bdaee-106">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="bdaee-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdaee-107">Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdaee-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="bdaee-108">Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="bdaee-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="bdaee-109">Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica.</span><span class="sxs-lookup"><span data-stu-id="bdaee-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="bdaee-110">Você pode criar, ler, atualizar e excluir as atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="bdaee-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bdaee-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdaee-111">JSON representation</span></span>

<span data-ttu-id="bdaee-112">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bdaee-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a><span data-ttu-id="bdaee-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdaee-113">Properties</span></span>
| <span data-ttu-id="bdaee-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdaee-114">Property</span></span>     | <span data-ttu-id="bdaee-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdaee-115">Type</span></span>   |<span data-ttu-id="bdaee-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdaee-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdaee-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="bdaee-117">creationTimestamp</span></span>|<span data-ttu-id="bdaee-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdaee-118">DateTimeOffset</span></span>|<span data-ttu-id="bdaee-119">A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: </span><span class="sxs-lookup"><span data-stu-id="bdaee-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bdaee-120">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bdaee-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bdaee-121">id</span><span class="sxs-lookup"><span data-stu-id="bdaee-121">id</span></span>|<span data-ttu-id="bdaee-122">Guid</span><span class="sxs-lookup"><span data-stu-id="bdaee-122">Guid</span></span>|<span data-ttu-id="bdaee-123">A ID de função que foi atribuída à entidade.</span><span class="sxs-lookup"><span data-stu-id="bdaee-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="bdaee-124">Essa função deve ser declarada pela **resourceId** do aplicativo do recurso de destino em sua propriedade **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="bdaee-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="bdaee-125">Quando o recurso não declarar nenhuma permissão, uma ID padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="bdaee-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="bdaee-126">Chave.</span><span class="sxs-lookup"><span data-stu-id="bdaee-126">Key.</span></span> <span data-ttu-id="bdaee-127">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="bdaee-127">Not nullable.</span></span> |
|<span data-ttu-id="bdaee-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdaee-128">principalDisplayName</span></span>|<span data-ttu-id="bdaee-129">String</span><span class="sxs-lookup"><span data-stu-id="bdaee-129">String</span></span>|<span data-ttu-id="bdaee-130">O nome de exibição da entidade à qual foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="bdaee-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="bdaee-131">principalId</span><span class="sxs-lookup"><span data-stu-id="bdaee-131">principalId</span></span>|<span data-ttu-id="bdaee-132">Guid</span><span class="sxs-lookup"><span data-stu-id="bdaee-132">Guid</span></span>|<span data-ttu-id="bdaee-133">O identificador exclusivo (**id**) da entidade à qual o acesso está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="bdaee-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="bdaee-134">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="bdaee-134">Required on create.</span></span>            |
|<span data-ttu-id="bdaee-135">principalType</span><span class="sxs-lookup"><span data-stu-id="bdaee-135">principalType</span></span>|<span data-ttu-id="bdaee-136">String</span><span class="sxs-lookup"><span data-stu-id="bdaee-136">String</span></span>|<span data-ttu-id="bdaee-137">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="bdaee-137">The type of principal.</span></span>  <span data-ttu-id="bdaee-138">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="bdaee-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="bdaee-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bdaee-139">resourceDisplayName</span></span>|<span data-ttu-id="bdaee-140">String</span><span class="sxs-lookup"><span data-stu-id="bdaee-140">String</span></span>|<span data-ttu-id="bdaee-141">O nome de exibição do recurso para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="bdaee-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="bdaee-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="bdaee-142">resourceId</span></span>|<span data-ttu-id="bdaee-143">Guid</span><span class="sxs-lookup"><span data-stu-id="bdaee-143">Guid</span></span>|<span data-ttu-id="bdaee-144">Identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="bdaee-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdaee-145">Relações</span><span class="sxs-lookup"><span data-stu-id="bdaee-145">Relationships</span></span>
<span data-ttu-id="bdaee-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bdaee-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="bdaee-147">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdaee-147">Methods</span></span>

| <span data-ttu-id="bdaee-148">Método</span><span class="sxs-lookup"><span data-stu-id="bdaee-148">Method</span></span>           | <span data-ttu-id="bdaee-149">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdaee-149">Return Type</span></span>    |<span data-ttu-id="bdaee-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdaee-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdaee-151">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bdaee-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="bdaee-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bdaee-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="bdaee-153">Leia propriedades e relações do objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="bdaee-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="bdaee-154">Update</span><span class="sxs-lookup"><span data-stu-id="bdaee-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="bdaee-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bdaee-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="bdaee-156">Atualize o objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="bdaee-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="bdaee-157">Delete</span><span class="sxs-lookup"><span data-stu-id="bdaee-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="bdaee-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdaee-158">None</span></span> |<span data-ttu-id="bdaee-159">Exclua o objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="bdaee-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
