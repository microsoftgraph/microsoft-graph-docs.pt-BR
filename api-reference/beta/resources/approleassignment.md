---
title: Tipo de recurso plannerAssignment
description: Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário. Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica. Você pode criar, ler, atualizar e excluir as atribuições de função.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5a0b9faeb68e11f465e8b5ddb177351e9a0f44d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508237"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="1441e-106">Tipo de recurso plannerAssignment</span><span class="sxs-lookup"><span data-stu-id="1441e-106">appRoleAssignment resource type</span></span>

<span data-ttu-id="1441e-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1441e-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1441e-108">Usado para registrar quando um usuário ou grupo é atribuído a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1441e-108">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="1441e-109">Nesse caso, a atribuição de função resultará em um bloco do aplicativo exibido no painel de acesso de aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="1441e-109">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="1441e-110">Essa entidade também pode ser usada para conceder a outro aplicativo (modelado como uma entidade de serviço) acesso a um aplicativo de recurso em uma função específica.</span><span class="sxs-lookup"><span data-stu-id="1441e-110">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="1441e-111">Você pode criar, ler, atualizar e excluir as atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="1441e-111">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1441e-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1441e-112">JSON representation</span></span>

<span data-ttu-id="1441e-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1441e-113">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="1441e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1441e-114">Properties</span></span>
| <span data-ttu-id="1441e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1441e-115">Property</span></span>     | <span data-ttu-id="1441e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="1441e-116">Type</span></span>   |<span data-ttu-id="1441e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="1441e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1441e-118">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="1441e-118">creationTimestamp</span></span>|<span data-ttu-id="1441e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1441e-119">DateTimeOffset</span></span>|<span data-ttu-id="1441e-120">A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: </span><span class="sxs-lookup"><span data-stu-id="1441e-120">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1441e-121">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1441e-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1441e-122">id</span><span class="sxs-lookup"><span data-stu-id="1441e-122">id</span></span>|<span data-ttu-id="1441e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="1441e-123">Guid</span></span>|<span data-ttu-id="1441e-124">A ID de função que foi atribuída à entidade.</span><span class="sxs-lookup"><span data-stu-id="1441e-124">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="1441e-125">Essa função deve ser declarada pela **resourceId** do aplicativo do recurso de destino em sua propriedade **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="1441e-125">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="1441e-126">Quando o recurso não declarar nenhuma permissão, uma ID padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="1441e-126">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="1441e-127">Chave.</span><span class="sxs-lookup"><span data-stu-id="1441e-127">Key.</span></span> <span data-ttu-id="1441e-128">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="1441e-128">Not nullable.</span></span> |
|<span data-ttu-id="1441e-129">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="1441e-129">principalDisplayName</span></span>|<span data-ttu-id="1441e-130">String</span><span class="sxs-lookup"><span data-stu-id="1441e-130">String</span></span>|<span data-ttu-id="1441e-131">O nome de exibição da entidade à qual foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="1441e-131">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="1441e-132">principalId</span><span class="sxs-lookup"><span data-stu-id="1441e-132">principalId</span></span>|<span data-ttu-id="1441e-133">Guid</span><span class="sxs-lookup"><span data-stu-id="1441e-133">Guid</span></span>|<span data-ttu-id="1441e-134">O identificador exclusivo (**id**) da entidade à qual o acesso está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="1441e-134">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="1441e-135">Obrigatório ao criar.</span><span class="sxs-lookup"><span data-stu-id="1441e-135">Required on create.</span></span>            |
|<span data-ttu-id="1441e-136">principalType</span><span class="sxs-lookup"><span data-stu-id="1441e-136">principalType</span></span>|<span data-ttu-id="1441e-137">String</span><span class="sxs-lookup"><span data-stu-id="1441e-137">String</span></span>|<span data-ttu-id="1441e-138">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="1441e-138">The type of principal.</span></span>  <span data-ttu-id="1441e-139">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="1441e-139">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="1441e-140">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1441e-140">resourceDisplayName</span></span>|<span data-ttu-id="1441e-141">String</span><span class="sxs-lookup"><span data-stu-id="1441e-141">String</span></span>|<span data-ttu-id="1441e-142">O nome de exibição do recurso para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="1441e-142">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="1441e-143">resourceId</span><span class="sxs-lookup"><span data-stu-id="1441e-143">resourceId</span></span>|<span data-ttu-id="1441e-144">Guid</span><span class="sxs-lookup"><span data-stu-id="1441e-144">Guid</span></span>|<span data-ttu-id="1441e-145">Identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="1441e-145">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1441e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="1441e-146">Relationships</span></span>
<span data-ttu-id="1441e-147">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1441e-147">None</span></span>


## <a name="methods"></a><span data-ttu-id="1441e-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="1441e-148">Methods</span></span>

| <span data-ttu-id="1441e-149">Método</span><span class="sxs-lookup"><span data-stu-id="1441e-149">Method</span></span>           | <span data-ttu-id="1441e-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1441e-150">Return Type</span></span>    |<span data-ttu-id="1441e-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="1441e-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1441e-152">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1441e-152">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="1441e-153">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1441e-153">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="1441e-154">Leia propriedades e relações do objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="1441e-154">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="1441e-155">Update</span><span class="sxs-lookup"><span data-stu-id="1441e-155">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="1441e-156">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1441e-156">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="1441e-157">Atualize o objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="1441e-157">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="1441e-158">Delete</span><span class="sxs-lookup"><span data-stu-id="1441e-158">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="1441e-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1441e-159">None</span></span> |<span data-ttu-id="1441e-160">Exclua o objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="1441e-160">Delete appRoleAssignment object.</span></span> |

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
