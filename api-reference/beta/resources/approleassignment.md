---
title: Tipo de recurso plannerAssignment
description: Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário. Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica. Você pode criar, ler, atualizar e excluir as atribuições de função.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 471927eb3aaf0dc26a3a70b0dffae7e15c812787
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974322"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="81ea0-106">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="81ea0-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ea0-107">Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81ea0-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="81ea0-108">Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="81ea0-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="81ea0-109">Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica.</span><span class="sxs-lookup"><span data-stu-id="81ea0-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="81ea0-110">Você pode criar, ler, atualizar e excluir as atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="81ea0-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="81ea0-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81ea0-111">JSON representation</span></span>

<span data-ttu-id="81ea0-112">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="81ea0-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
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
## <a name="properties"></a><span data-ttu-id="81ea0-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81ea0-113">Properties</span></span>
| <span data-ttu-id="81ea0-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81ea0-114">Property</span></span>     | <span data-ttu-id="81ea0-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="81ea0-115">Type</span></span>   |<span data-ttu-id="81ea0-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ea0-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81ea0-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="81ea0-117">creationTimestamp</span></span>|<span data-ttu-id="81ea0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ea0-118">DateTimeOffset</span></span>|<span data-ttu-id="81ea0-119">A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: </span><span class="sxs-lookup"><span data-stu-id="81ea0-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81ea0-120">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="81ea0-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="81ea0-121">id</span><span class="sxs-lookup"><span data-stu-id="81ea0-121">id</span></span>|<span data-ttu-id="81ea0-122">Guid</span><span class="sxs-lookup"><span data-stu-id="81ea0-122">Guid</span></span>|<span data-ttu-id="81ea0-123">A ID de função que foi atribuída à entidade.</span><span class="sxs-lookup"><span data-stu-id="81ea0-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="81ea0-124">Essa função deve ser declarada pela **resourceId** do aplicativo do recurso de destino em sua propriedade **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="81ea0-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="81ea0-125">Quando o recurso não declarar nenhuma permissão, uma ID padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="81ea0-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="81ea0-126">Chave.</span><span class="sxs-lookup"><span data-stu-id="81ea0-126">Key.</span></span> <span data-ttu-id="81ea0-127">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="81ea0-127">Not nullable.</span></span> |
|<span data-ttu-id="81ea0-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="81ea0-128">principalDisplayName</span></span>|<span data-ttu-id="81ea0-129">String</span><span class="sxs-lookup"><span data-stu-id="81ea0-129">String</span></span>|<span data-ttu-id="81ea0-130">O nome de exibição da entidade à qual foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="81ea0-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="81ea0-131">principalId</span><span class="sxs-lookup"><span data-stu-id="81ea0-131">principalId</span></span>|<span data-ttu-id="81ea0-132">Guid</span><span class="sxs-lookup"><span data-stu-id="81ea0-132">Guid</span></span>|<span data-ttu-id="81ea0-133">O identificador exclusivo (**id**) da entidade à qual o acesso está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="81ea0-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="81ea0-134">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="81ea0-134">Required on create.</span></span>            |
|<span data-ttu-id="81ea0-135">principalType</span><span class="sxs-lookup"><span data-stu-id="81ea0-135">principalType</span></span>|<span data-ttu-id="81ea0-136">String</span><span class="sxs-lookup"><span data-stu-id="81ea0-136">String</span></span>|<span data-ttu-id="81ea0-137">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="81ea0-137">The type of principal.</span></span>  <span data-ttu-id="81ea0-138">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="81ea0-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="81ea0-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="81ea0-139">resourceDisplayName</span></span>|<span data-ttu-id="81ea0-140">String</span><span class="sxs-lookup"><span data-stu-id="81ea0-140">String</span></span>|<span data-ttu-id="81ea0-141">O nome de exibição do recurso para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="81ea0-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="81ea0-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="81ea0-142">resourceId</span></span>|<span data-ttu-id="81ea0-143">Guid</span><span class="sxs-lookup"><span data-stu-id="81ea0-143">Guid</span></span>|<span data-ttu-id="81ea0-144">Identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="81ea0-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81ea0-145">Relações</span><span class="sxs-lookup"><span data-stu-id="81ea0-145">Relationships</span></span>
<span data-ttu-id="81ea0-146">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="81ea0-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="81ea0-147">Métodos</span><span class="sxs-lookup"><span data-stu-id="81ea0-147">Methods</span></span>

| <span data-ttu-id="81ea0-148">Método</span><span class="sxs-lookup"><span data-stu-id="81ea0-148">Method</span></span>           | <span data-ttu-id="81ea0-149">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81ea0-149">Return Type</span></span>    |<span data-ttu-id="81ea0-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ea0-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81ea0-151">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81ea0-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="81ea0-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81ea0-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="81ea0-153">Leia propriedades e relações do objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="81ea0-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="81ea0-154">Update</span><span class="sxs-lookup"><span data-stu-id="81ea0-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="81ea0-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81ea0-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="81ea0-156">Atualize o objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="81ea0-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="81ea0-157">Delete</span><span class="sxs-lookup"><span data-stu-id="81ea0-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="81ea0-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81ea0-158">None</span></span> |<span data-ttu-id="81ea0-159">Exclua o objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="81ea0-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
