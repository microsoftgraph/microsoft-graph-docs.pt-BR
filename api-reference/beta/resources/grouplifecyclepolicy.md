---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida para um grupo do Microsoft 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d01be98869a62d72b275f5840ddc2e0edcd5c698
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078427"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="8ddec-103">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="8ddec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ddec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ddec-105">Representa uma política de ciclo de vida para um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8ddec-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="8ddec-106">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="8ddec-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="8ddec-107">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="8ddec-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="8ddec-108">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8ddec-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="8ddec-109">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="8ddec-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="8ddec-110">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="8ddec-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="8ddec-111">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="8ddec-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="8ddec-112">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="8ddec-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="8ddec-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ddec-113">Methods</span></span>

| <span data-ttu-id="8ddec-114">Método</span><span class="sxs-lookup"><span data-stu-id="8ddec-114">Method</span></span> | <span data-ttu-id="8ddec-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ddec-115">Return Type</span></span> | <span data-ttu-id="8ddec-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddec-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ddec-117">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="8ddec-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="8ddec-119">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8ddec-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="8ddec-120">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="8ddec-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="8ddec-121">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ddec-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="8ddec-122">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="8ddec-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="8ddec-123">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="8ddec-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="8ddec-125">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8ddec-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="8ddec-126">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="8ddec-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddec-127">None</span></span> | <span data-ttu-id="8ddec-128">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="8ddec-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="8ddec-129">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="8ddec-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddec-130">None</span></span>| <span data-ttu-id="8ddec-131">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="8ddec-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="8ddec-132">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="8ddec-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="8ddec-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddec-133">None</span></span>| <span data-ttu-id="8ddec-134">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="8ddec-134">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="8ddec-135">Renovar um grupo</span><span class="sxs-lookup"><span data-stu-id="8ddec-135">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="8ddec-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddec-136">None</span></span>| <span data-ttu-id="8ddec-137">Renovar a data de vencimento de um grupo.</span><span class="sxs-lookup"><span data-stu-id="8ddec-137">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ddec-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ddec-138">Properties</span></span>

| <span data-ttu-id="8ddec-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ddec-139">Property</span></span> | <span data-ttu-id="8ddec-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ddec-140">Type</span></span> | <span data-ttu-id="8ddec-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddec-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8ddec-142">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="8ddec-142">alternateNotificationEmails</span></span>|<span data-ttu-id="8ddec-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddec-143">String</span></span>| <span data-ttu-id="8ddec-144">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="8ddec-144">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="8ddec-145">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="8ddec-145">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="8ddec-146">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="8ddec-146">groupLifetimeInDays</span></span>|<span data-ttu-id="8ddec-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8ddec-147">Int32</span></span>| <span data-ttu-id="8ddec-148">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="8ddec-148">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="8ddec-149">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="8ddec-149">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="8ddec-150">id</span><span class="sxs-lookup"><span data-stu-id="8ddec-150">id</span></span>|<span data-ttu-id="8ddec-151">Guid</span><span class="sxs-lookup"><span data-stu-id="8ddec-151">Guid</span></span>| <span data-ttu-id="8ddec-152">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="8ddec-152">A unique identifier for a policy.</span></span> <span data-ttu-id="8ddec-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ddec-153">Read-only.</span></span>|
|<span data-ttu-id="8ddec-154">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="8ddec-154">managedGroupTypes</span></span>|<span data-ttu-id="8ddec-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddec-155">String</span></span>| <span data-ttu-id="8ddec-156">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="8ddec-156">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="8ddec-157">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="8ddec-157">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ddec-158">Relações</span><span class="sxs-lookup"><span data-stu-id="8ddec-158">Relationships</span></span>

<span data-ttu-id="8ddec-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddec-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ddec-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ddec-160">JSON representation</span></span>

<span data-ttu-id="8ddec-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ddec-161">Here is a JSON representation of the resource.</span></span>

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


