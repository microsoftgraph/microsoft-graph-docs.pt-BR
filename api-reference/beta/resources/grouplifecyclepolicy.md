---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida de um Grupo do Office 365. Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos. Por exemplo, após 180 dias o grupo expira. Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador. Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política. Por exemplo, a nova validade do grupo é de 180 dias após a renovação. Caso não seja renovado, ele expirará e será excluído. É possível renovar o grupo no prazo de 30 dias da data de exclusão.
ms.openlocfilehash: c4a4d5b495f3bbb0d0c55b61a259f2105d0fea9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036581"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="96971-110">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="96971-111">Representa uma política de ciclo de vida de um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="96971-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="96971-112">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="96971-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="96971-113">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="96971-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="96971-114">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="96971-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="96971-115">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="96971-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="96971-116">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="96971-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="96971-117">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="96971-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="96971-118">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="96971-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="96971-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="96971-119">Methods</span></span>

| <span data-ttu-id="96971-120">Método</span><span class="sxs-lookup"><span data-stu-id="96971-120">Method</span></span> | <span data-ttu-id="96971-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96971-121">Return Type</span></span> | <span data-ttu-id="96971-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96971-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="96971-123">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="96971-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="96971-125">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="96971-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="96971-126">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="96971-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="96971-127">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="96971-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="96971-128">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="96971-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="96971-129">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="96971-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="96971-131">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="96971-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="96971-132">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="96971-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96971-133">None</span></span> | <span data-ttu-id="96971-134">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="96971-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="96971-135">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="96971-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96971-136">None</span></span>| <span data-ttu-id="96971-137">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="96971-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="96971-138">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="96971-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="96971-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96971-139">None</span></span>| <span data-ttu-id="96971-140">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="96971-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="96971-141">Renovar um grupo</span><span class="sxs-lookup"><span data-stu-id="96971-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="96971-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96971-142">None</span></span>| <span data-ttu-id="96971-143">Renove a data de validade de um grupo.</span><span class="sxs-lookup"><span data-stu-id="96971-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="96971-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96971-144">Properties</span></span>

| <span data-ttu-id="96971-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96971-145">Property</span></span> | <span data-ttu-id="96971-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="96971-146">Type</span></span> | <span data-ttu-id="96971-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="96971-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="96971-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="96971-148">alternateNotificationEmails</span></span>|<span data-ttu-id="96971-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96971-149">String</span></span>| <span data-ttu-id="96971-150">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="96971-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="96971-151">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="96971-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="96971-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="96971-152">groupLifetimeInDays</span></span>|<span data-ttu-id="96971-153">Int32</span><span class="sxs-lookup"><span data-stu-id="96971-153">Int32</span></span>| <span data-ttu-id="96971-154">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="96971-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="96971-155">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="96971-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="96971-156">id</span><span class="sxs-lookup"><span data-stu-id="96971-156">id</span></span>|<span data-ttu-id="96971-157">Guid</span><span class="sxs-lookup"><span data-stu-id="96971-157">Guid</span></span>| <span data-ttu-id="96971-158">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="96971-158">A unique identifier for a policy.</span></span> <span data-ttu-id="96971-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96971-159">Read-only.</span></span>|
|<span data-ttu-id="96971-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="96971-160">managedGroupTypes</span></span>|<span data-ttu-id="96971-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96971-161">String</span></span>| <span data-ttu-id="96971-162">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="96971-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="96971-163">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="96971-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96971-164">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="96971-164">Relationships</span></span>

<span data-ttu-id="96971-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96971-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96971-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96971-166">JSON representation</span></span>

<span data-ttu-id="96971-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96971-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->