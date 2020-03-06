---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida de um grupo do Office 365. Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos. Por exemplo, após 180 dias o grupo expira. Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador. Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política. Por exemplo, a nova validade do grupo é de 180 dias após a renovação. Caso não seja renovado, ele expirará e será excluído. É possível renovar o grupo no prazo de 30 dias da data de exclusão.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: acd1e2b8b66d7cb643e483ee099a3c9909df5d9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532921"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="f05d6-110">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="f05d6-111">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f05d6-111">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f05d6-112">Representa uma política de ciclo de vida de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f05d6-112">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="f05d6-113">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="f05d6-113">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="f05d6-114">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="f05d6-114">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="f05d6-115">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f05d6-115">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="f05d6-116">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="f05d6-116">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="f05d6-117">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="f05d6-117">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="f05d6-118">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="f05d6-118">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="f05d6-119">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="f05d6-119">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="f05d6-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="f05d6-120">Methods</span></span>

| <span data-ttu-id="f05d6-121">Método</span><span class="sxs-lookup"><span data-stu-id="f05d6-121">Method</span></span> | <span data-ttu-id="f05d6-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f05d6-122">Return Type</span></span> | <span data-ttu-id="f05d6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f05d6-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f05d6-124">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-124">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="f05d6-125">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-125">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="f05d6-126">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="f05d6-126">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="f05d6-127">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="f05d6-127">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="f05d6-128">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f05d6-128">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="f05d6-129">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="f05d6-129">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="f05d6-130">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-130">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="f05d6-131">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-131">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="f05d6-132">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="f05d6-132">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="f05d6-133">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-133">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="f05d6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f05d6-134">None</span></span> | <span data-ttu-id="f05d6-135">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="f05d6-135">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="f05d6-136">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-136">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="f05d6-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f05d6-137">None</span></span>| <span data-ttu-id="f05d6-138">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="f05d6-138">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="f05d6-139">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f05d6-139">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="f05d6-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f05d6-140">None</span></span>| <span data-ttu-id="f05d6-141">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f05d6-141">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="f05d6-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f05d6-142">Properties</span></span>

| <span data-ttu-id="f05d6-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f05d6-143">Property</span></span> | <span data-ttu-id="f05d6-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="f05d6-144">Type</span></span> | <span data-ttu-id="f05d6-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="f05d6-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f05d6-146">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f05d6-146">alternateNotificationEmails</span></span>|<span data-ttu-id="f05d6-147">String</span><span class="sxs-lookup"><span data-stu-id="f05d6-147">String</span></span>| <span data-ttu-id="f05d6-148">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="f05d6-148">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="f05d6-149">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="f05d6-149">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="f05d6-150">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="f05d6-150">groupLifetimeInDays</span></span>|<span data-ttu-id="f05d6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f05d6-151">Int32</span></span>| <span data-ttu-id="f05d6-152">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="f05d6-152">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="f05d6-153">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="f05d6-153">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="f05d6-154">id</span><span class="sxs-lookup"><span data-stu-id="f05d6-154">id</span></span>|<span data-ttu-id="f05d6-155">Guid</span><span class="sxs-lookup"><span data-stu-id="f05d6-155">Guid</span></span>| <span data-ttu-id="f05d6-156">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="f05d6-156">A unique identifier for a policy.</span></span> <span data-ttu-id="f05d6-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f05d6-157">Read-only.</span></span>|
|<span data-ttu-id="f05d6-158">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="f05d6-158">managedGroupTypes</span></span>|<span data-ttu-id="f05d6-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f05d6-159">String</span></span>| <span data-ttu-id="f05d6-160">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="f05d6-160">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="f05d6-161">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="f05d6-161">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f05d6-162">Relações</span><span class="sxs-lookup"><span data-stu-id="f05d6-162">Relationships</span></span>

<span data-ttu-id="f05d6-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f05d6-163">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f05d6-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f05d6-164">JSON representation</span></span>

<span data-ttu-id="f05d6-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f05d6-165">Here is a JSON representation of the resource.</span></span>

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
