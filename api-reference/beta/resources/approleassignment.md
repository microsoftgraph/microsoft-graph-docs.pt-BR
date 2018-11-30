---
title: tipo de recurso de appRoleAssignment
description: Usado para registrar quando um usuário ou grupo for atribuído a um aplicativo. Nesse caso, a atribuição de função resultará em um elemento de aplicativo aparecendo backup na painel de acesso do aplicativo do usuário. Esta entidade também pode ser usada para conceder acesso de outro aplicativo (modelado como uma entidade de serviço) para um aplicativo de recursos em uma determinada função. Você pode criar, ler, atualizar e excluir atribuições de função.
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034600"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="816cc-106">tipo de recurso de appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="816cc-106">appRoleAssignment resource type</span></span>

> <span data-ttu-id="816cc-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="816cc-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="816cc-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="816cc-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="816cc-109">Usado para registrar quando um usuário ou grupo for atribuído a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="816cc-109">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="816cc-110">Nesse caso, a atribuição de função resultará em um elemento de aplicativo aparecendo backup na painel de acesso do aplicativo do usuário.</span><span class="sxs-lookup"><span data-stu-id="816cc-110">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="816cc-111">Esta entidade também pode ser usada para conceder acesso de outro aplicativo (modelado como uma entidade de serviço) para um aplicativo de recursos em uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="816cc-111">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="816cc-112">Você pode criar, ler, atualizar e excluir atribuições de função.</span><span class="sxs-lookup"><span data-stu-id="816cc-112">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="816cc-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="816cc-113">JSON representation</span></span>

<span data-ttu-id="816cc-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="816cc-114">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="816cc-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="816cc-115">Properties</span></span>
| <span data-ttu-id="816cc-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="816cc-116">Property</span></span>     | <span data-ttu-id="816cc-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="816cc-117">Type</span></span>   |<span data-ttu-id="816cc-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="816cc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="816cc-119">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="816cc-119">creationTimestamp</span></span>|<span data-ttu-id="816cc-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="816cc-120">DateTimeOffset</span></span>|<span data-ttu-id="816cc-121">A hora em que a concessão foi criada. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="816cc-121">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="816cc-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="816cc-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="816cc-123">id</span><span class="sxs-lookup"><span data-stu-id="816cc-123">id</span></span>|<span data-ttu-id="816cc-124">Guid</span><span class="sxs-lookup"><span data-stu-id="816cc-124">Guid</span></span>|<span data-ttu-id="816cc-125">A id de função que foi atribuída à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="816cc-125">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="816cc-126">Essa função deve ser declarada pelo destino recurso aplicativo **resourceId** em sua propriedade **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="816cc-126">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="816cc-127">Onde o recurso não declarar todas as permissões, uma id do padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="816cc-127">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="816cc-128">Chave.</span><span class="sxs-lookup"><span data-stu-id="816cc-128">Key.</span></span> <span data-ttu-id="816cc-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="816cc-129">Not nullable.</span></span> |
|<span data-ttu-id="816cc-130">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="816cc-130">principalDisplayName</span></span>|<span data-ttu-id="816cc-131">String</span><span class="sxs-lookup"><span data-stu-id="816cc-131">String</span></span>|<span data-ttu-id="816cc-132">O nome de exibição da entidade que foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="816cc-132">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="816cc-133">principalId</span><span class="sxs-lookup"><span data-stu-id="816cc-133">principalId</span></span>|<span data-ttu-id="816cc-134">Guid</span><span class="sxs-lookup"><span data-stu-id="816cc-134">Guid</span></span>|<span data-ttu-id="816cc-135">O identificador exclusivo (**id**) para a entidade sendo concedida o acesso.</span><span class="sxs-lookup"><span data-stu-id="816cc-135">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="816cc-136">Necessários na criação.</span><span class="sxs-lookup"><span data-stu-id="816cc-136">Required on create.</span></span>            |
|<span data-ttu-id="816cc-137">principalType</span><span class="sxs-lookup"><span data-stu-id="816cc-137">principalType</span></span>|<span data-ttu-id="816cc-138">String</span><span class="sxs-lookup"><span data-stu-id="816cc-138">String</span></span>|<span data-ttu-id="816cc-139">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="816cc-139">The type of principal.</span></span>  <span data-ttu-id="816cc-140">Isso pode ser "User", "Grupo" ou "ServicePrincipal".</span><span class="sxs-lookup"><span data-stu-id="816cc-140">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="816cc-141">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="816cc-141">resourceDisplayName</span></span>|<span data-ttu-id="816cc-142">String</span><span class="sxs-lookup"><span data-stu-id="816cc-142">String</span></span>|<span data-ttu-id="816cc-143">O nome de exibição do recurso para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="816cc-143">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="816cc-144">resourceId</span><span class="sxs-lookup"><span data-stu-id="816cc-144">resourceId</span></span>|<span data-ttu-id="816cc-145">Guid</span><span class="sxs-lookup"><span data-stu-id="816cc-145">Guid</span></span>|<span data-ttu-id="816cc-146">O identificador exclusivo (**id**) para o recurso de destino (entidade de serviço) para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="816cc-146">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="816cc-147">Relações</span><span class="sxs-lookup"><span data-stu-id="816cc-147">Relationships</span></span>
<span data-ttu-id="816cc-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="816cc-148">None</span></span>


## <a name="methods"></a><span data-ttu-id="816cc-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="816cc-149">Methods</span></span>

| <span data-ttu-id="816cc-150">Método</span><span class="sxs-lookup"><span data-stu-id="816cc-150">Method</span></span>           | <span data-ttu-id="816cc-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="816cc-151">Return Type</span></span>    |<span data-ttu-id="816cc-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="816cc-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="816cc-153">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="816cc-153">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="816cc-154">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="816cc-154">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="816cc-155">Leia as propriedades e os relacionamentos do objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="816cc-155">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="816cc-156">Update</span><span class="sxs-lookup"><span data-stu-id="816cc-156">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="816cc-157">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="816cc-157">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="816cc-158">Atualize o objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="816cc-158">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="816cc-159">Delete</span><span class="sxs-lookup"><span data-stu-id="816cc-159">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="816cc-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="816cc-160">None</span></span> |<span data-ttu-id="816cc-161">Exclua objeto appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="816cc-161">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->