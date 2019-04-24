---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida de um Grupo do Office 365. Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos. Por exemplo, após 180 dias o grupo expira. Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador. Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política. Por exemplo, a nova validade do grupo é de 180 dias após a renovação. Caso não seja renovado, ele expirará e será excluído. É possível renovar o grupo no prazo de 30 dias da data de exclusão.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c69a54ef5323b1e3d171135d4b1b0231b6834c79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506353"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="56ba5-110">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="56ba5-111">Representa uma política de ciclo de vida de um Grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="56ba5-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="56ba5-112">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="56ba5-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="56ba5-113">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="56ba5-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="56ba5-114">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="56ba5-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="56ba5-115">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="56ba5-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="56ba5-116">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="56ba5-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="56ba5-117">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="56ba5-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="56ba5-118">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="56ba5-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="56ba5-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="56ba5-119">Methods</span></span>

| <span data-ttu-id="56ba5-120">Método</span><span class="sxs-lookup"><span data-stu-id="56ba5-120">Method</span></span> | <span data-ttu-id="56ba5-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56ba5-121">Return Type</span></span> | <span data-ttu-id="56ba5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ba5-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="56ba5-123">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="56ba5-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="56ba5-125">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="56ba5-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="56ba5-126">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="56ba5-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="56ba5-127">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56ba5-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="56ba5-128">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="56ba5-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="56ba5-129">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="56ba5-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="56ba5-131">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="56ba5-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="56ba5-132">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="56ba5-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56ba5-133">None</span></span> | <span data-ttu-id="56ba5-134">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="56ba5-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="56ba5-135">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="56ba5-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56ba5-136">None</span></span>| <span data-ttu-id="56ba5-137">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="56ba5-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="56ba5-138">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="56ba5-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="56ba5-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56ba5-139">None</span></span>| <span data-ttu-id="56ba5-140">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="56ba5-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="56ba5-141">ReNovar um grupo</span><span class="sxs-lookup"><span data-stu-id="56ba5-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="56ba5-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56ba5-142">None</span></span>| <span data-ttu-id="56ba5-143">ReNovar a data de vencimento de um grupo.</span><span class="sxs-lookup"><span data-stu-id="56ba5-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="56ba5-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56ba5-144">Properties</span></span>

| <span data-ttu-id="56ba5-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56ba5-145">Property</span></span> | <span data-ttu-id="56ba5-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ba5-146">Type</span></span> | <span data-ttu-id="56ba5-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ba5-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="56ba5-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="56ba5-148">alternateNotificationEmails</span></span>|<span data-ttu-id="56ba5-149">String</span><span class="sxs-lookup"><span data-stu-id="56ba5-149">String</span></span>| <span data-ttu-id="56ba5-150">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="56ba5-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="56ba5-151">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="56ba5-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="56ba5-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="56ba5-152">groupLifetimeInDays</span></span>|<span data-ttu-id="56ba5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="56ba5-153">Int32</span></span>| <span data-ttu-id="56ba5-154">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="56ba5-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="56ba5-155">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="56ba5-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="56ba5-156">id</span><span class="sxs-lookup"><span data-stu-id="56ba5-156">id</span></span>|<span data-ttu-id="56ba5-157">Guid</span><span class="sxs-lookup"><span data-stu-id="56ba5-157">Guid</span></span>| <span data-ttu-id="56ba5-158">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="56ba5-158">A unique identifier for a policy.</span></span> <span data-ttu-id="56ba5-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56ba5-159">Read-only.</span></span>|
|<span data-ttu-id="56ba5-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="56ba5-160">managedGroupTypes</span></span>|<span data-ttu-id="56ba5-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56ba5-161">String</span></span>| <span data-ttu-id="56ba5-162">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="56ba5-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="56ba5-163">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="56ba5-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="56ba5-164">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="56ba5-164">Relationships</span></span>

<span data-ttu-id="56ba5-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56ba5-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56ba5-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56ba5-166">JSON representation</span></span>

<span data-ttu-id="56ba5-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56ba5-167">Here is a JSON representation of the resource.</span></span>

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
