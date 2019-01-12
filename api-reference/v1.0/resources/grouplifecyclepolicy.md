---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida de um Grupo do Office 365. Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos. Por exemplo, após 180 dias o grupo expira. Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador. Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política. Por exemplo, a nova validade do grupo é de 180 dias após a renovação. Caso não seja renovado, ele expirará e será excluído. É possível renovar o grupo no prazo de 30 dias da data de exclusão.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 65cf8d5d06262f1d5700de26b4c4f62b005020d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964162"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="8c450-110">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="8c450-111">Representa uma política de ciclo de vida de um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8c450-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="8c450-112">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="8c450-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="8c450-113">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="8c450-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="8c450-114">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8c450-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="8c450-115">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="8c450-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="8c450-116">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="8c450-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="8c450-117">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="8c450-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="8c450-118">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="8c450-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="8c450-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="8c450-119">Methods</span></span>

| <span data-ttu-id="8c450-120">Método</span><span class="sxs-lookup"><span data-stu-id="8c450-120">Method</span></span> | <span data-ttu-id="8c450-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8c450-121">Return Type</span></span> | <span data-ttu-id="8c450-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c450-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c450-123">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="8c450-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="8c450-125">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8c450-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="8c450-126">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="8c450-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="8c450-127">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8c450-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="8c450-128">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="8c450-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="8c450-129">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="8c450-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="8c450-131">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8c450-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="8c450-132">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="8c450-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c450-133">None</span></span> | <span data-ttu-id="8c450-134">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8c450-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="8c450-135">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="8c450-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c450-136">None</span></span>| <span data-ttu-id="8c450-137">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="8c450-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="8c450-138">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8c450-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="8c450-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c450-139">None</span></span>| <span data-ttu-id="8c450-140">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="8c450-140">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="8c450-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c450-141">Properties</span></span>

| <span data-ttu-id="8c450-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c450-142">Property</span></span> | <span data-ttu-id="8c450-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c450-143">Type</span></span> | <span data-ttu-id="8c450-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c450-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8c450-145">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="8c450-145">alternateNotificationEmails</span></span>|<span data-ttu-id="8c450-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c450-146">String</span></span>| <span data-ttu-id="8c450-147">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="8c450-147">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="8c450-148">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="8c450-148">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="8c450-149">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="8c450-149">groupLifetimeInDays</span></span>|<span data-ttu-id="8c450-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8c450-150">Int32</span></span>| <span data-ttu-id="8c450-151">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="8c450-151">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="8c450-152">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="8c450-152">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="8c450-153">id</span><span class="sxs-lookup"><span data-stu-id="8c450-153">id</span></span>|<span data-ttu-id="8c450-154">Guid</span><span class="sxs-lookup"><span data-stu-id="8c450-154">Guid</span></span>| <span data-ttu-id="8c450-155">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="8c450-155">A unique identifier for a policy.</span></span> <span data-ttu-id="8c450-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8c450-156">Read-only.</span></span>|
|<span data-ttu-id="8c450-157">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="8c450-157">managedGroupTypes</span></span>|<span data-ttu-id="8c450-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c450-158">String</span></span>| <span data-ttu-id="8c450-159">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="8c450-159">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="8c450-160">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="8c450-160">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8c450-161">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="8c450-161">Relationships</span></span>

<span data-ttu-id="8c450-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c450-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c450-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c450-163">JSON representation</span></span>

<span data-ttu-id="8c450-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c450-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
