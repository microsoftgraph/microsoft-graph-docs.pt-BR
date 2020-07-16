---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida para um grupo do Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b99e79da21f7aefe523b7bebe27115d9d38d4b55
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895500"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="198a7-103">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="198a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="198a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="198a7-105">Representa uma política de ciclo de vida para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="198a7-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="198a7-106">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="198a7-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="198a7-107">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="198a7-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="198a7-108">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="198a7-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="198a7-109">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="198a7-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="198a7-110">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="198a7-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="198a7-111">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="198a7-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="198a7-112">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="198a7-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="198a7-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="198a7-113">Methods</span></span>

| <span data-ttu-id="198a7-114">Método</span><span class="sxs-lookup"><span data-stu-id="198a7-114">Method</span></span> | <span data-ttu-id="198a7-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="198a7-115">Return Type</span></span> | <span data-ttu-id="198a7-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="198a7-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="198a7-117">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="198a7-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="198a7-119">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="198a7-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="198a7-120">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="198a7-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="198a7-121">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="198a7-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="198a7-122">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="198a7-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="198a7-123">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="198a7-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="198a7-125">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="198a7-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="198a7-126">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="198a7-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198a7-127">None</span></span> | <span data-ttu-id="198a7-128">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="198a7-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="198a7-129">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="198a7-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198a7-130">None</span></span>| <span data-ttu-id="198a7-131">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="198a7-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="198a7-132">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="198a7-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="198a7-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198a7-133">None</span></span>| <span data-ttu-id="198a7-134">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="198a7-134">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="198a7-135">Renovar um grupo</span><span class="sxs-lookup"><span data-stu-id="198a7-135">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="198a7-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198a7-136">None</span></span>| <span data-ttu-id="198a7-137">Renovar a data de vencimento de um grupo.</span><span class="sxs-lookup"><span data-stu-id="198a7-137">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="198a7-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="198a7-138">Properties</span></span>

| <span data-ttu-id="198a7-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="198a7-139">Property</span></span> | <span data-ttu-id="198a7-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="198a7-140">Type</span></span> | <span data-ttu-id="198a7-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="198a7-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="198a7-142">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="198a7-142">alternateNotificationEmails</span></span>|<span data-ttu-id="198a7-143">String</span><span class="sxs-lookup"><span data-stu-id="198a7-143">String</span></span>| <span data-ttu-id="198a7-144">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="198a7-144">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="198a7-145">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="198a7-145">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="198a7-146">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="198a7-146">groupLifetimeInDays</span></span>|<span data-ttu-id="198a7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="198a7-147">Int32</span></span>| <span data-ttu-id="198a7-148">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="198a7-148">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="198a7-149">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="198a7-149">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="198a7-150">id</span><span class="sxs-lookup"><span data-stu-id="198a7-150">id</span></span>|<span data-ttu-id="198a7-151">Guid</span><span class="sxs-lookup"><span data-stu-id="198a7-151">Guid</span></span>| <span data-ttu-id="198a7-152">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="198a7-152">A unique identifier for a policy.</span></span> <span data-ttu-id="198a7-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="198a7-153">Read-only.</span></span>|
|<span data-ttu-id="198a7-154">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="198a7-154">managedGroupTypes</span></span>|<span data-ttu-id="198a7-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="198a7-155">String</span></span>| <span data-ttu-id="198a7-156">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="198a7-156">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="198a7-157">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="198a7-157">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="198a7-158">Relações</span><span class="sxs-lookup"><span data-stu-id="198a7-158">Relationships</span></span>

<span data-ttu-id="198a7-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198a7-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="198a7-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="198a7-160">JSON representation</span></span>

<span data-ttu-id="198a7-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="198a7-161">Here is a JSON representation of the resource.</span></span>

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
