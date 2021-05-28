---
title: Tipo de recurso groupLifecyclePolicy
description: Representa uma política de ciclo de vida para um Microsoft 365 grupo.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: da3fa558df864f3dd0683ae4aaa08234c9ebd158
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680093"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="ab58a-103">Tipo de recurso groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="ab58a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab58a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab58a-105">Representa uma política de ciclo de vida para um Microsoft 365 grupo.</span><span class="sxs-lookup"><span data-stu-id="ab58a-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="ab58a-106">Uma política de ciclo de vida permite aos administradores definir um período de validade para os grupos.</span><span class="sxs-lookup"><span data-stu-id="ab58a-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="ab58a-107">Por exemplo, após 180 dias o grupo expira.</span><span class="sxs-lookup"><span data-stu-id="ab58a-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="ab58a-108">Quando um grupo alcança esse prazo, os proprietários devem renovar o grupo por um período definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ab58a-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="ab58a-109">Depois de renovado, o período de validade é estendido de acordo com o número de dias definido na política.</span><span class="sxs-lookup"><span data-stu-id="ab58a-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="ab58a-110">Por exemplo, a nova validade do grupo é de 180 dias após a renovação.</span><span class="sxs-lookup"><span data-stu-id="ab58a-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="ab58a-111">Caso não seja renovado, ele expirará e será excluído.</span><span class="sxs-lookup"><span data-stu-id="ab58a-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="ab58a-112">É possível renovar o grupo no prazo de 30 dias da data de exclusão.</span><span class="sxs-lookup"><span data-stu-id="ab58a-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="ab58a-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab58a-113">Methods</span></span>

| <span data-ttu-id="ab58a-114">Método</span><span class="sxs-lookup"><span data-stu-id="ab58a-114">Method</span></span> | <span data-ttu-id="ab58a-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab58a-115">Return Type</span></span> | <span data-ttu-id="ab58a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab58a-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab58a-117">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="ab58a-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="ab58a-119">Leia as propriedades e os relacionamentos de um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="ab58a-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="ab58a-120">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="ab58a-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="ab58a-121">Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ab58a-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="ab58a-122">Listar todos os objetos groupLifecyclePolicies.</span><span class="sxs-lookup"><span data-stu-id="ab58a-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="ab58a-123">Atualizar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="ab58a-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="ab58a-125">Atualizar um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="ab58a-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="ab58a-126">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="ab58a-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab58a-127">None</span></span> | <span data-ttu-id="ab58a-128">Excluir um objeto groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="ab58a-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="ab58a-129">Adicionar um grupo a um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="ab58a-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab58a-130">None</span></span>| <span data-ttu-id="ab58a-131">Adicionar um grupo a uma política de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="ab58a-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="ab58a-132">Remover um grupo de um objeto groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ab58a-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="ab58a-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab58a-133">None</span></span>| <span data-ttu-id="ab58a-134">Remover um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="ab58a-134">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab58a-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab58a-135">Properties</span></span>

| <span data-ttu-id="ab58a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab58a-136">Property</span></span> | <span data-ttu-id="ab58a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab58a-137">Type</span></span> | <span data-ttu-id="ab58a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab58a-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ab58a-139">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="ab58a-139">alternateNotificationEmails</span></span>|<span data-ttu-id="ab58a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab58a-140">String</span></span>| <span data-ttu-id="ab58a-141">Lista de endereços de email para o envio de notificações para grupos sem proprietários.</span><span class="sxs-lookup"><span data-stu-id="ab58a-141">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="ab58a-142">É possível definir vários endereços de email separando-os com ponto-e-vírgula.</span><span class="sxs-lookup"><span data-stu-id="ab58a-142">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="ab58a-143">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="ab58a-143">groupLifetimeInDays</span></span>|<span data-ttu-id="ab58a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ab58a-144">Int32</span></span>| <span data-ttu-id="ab58a-145">Número de dias antes que um grupo expire e precise ser renovado.</span><span class="sxs-lookup"><span data-stu-id="ab58a-145">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="ab58a-146">Após renová-lo, o período de validade é estendido de acordo com o número de dias definido.</span><span class="sxs-lookup"><span data-stu-id="ab58a-146">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="ab58a-147">id</span><span class="sxs-lookup"><span data-stu-id="ab58a-147">id</span></span>|<span data-ttu-id="ab58a-148">Guid</span><span class="sxs-lookup"><span data-stu-id="ab58a-148">Guid</span></span>| <span data-ttu-id="ab58a-149">Um identificador exclusivo de uma política.</span><span class="sxs-lookup"><span data-stu-id="ab58a-149">A unique identifier for a policy.</span></span> <span data-ttu-id="ab58a-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab58a-150">Read-only.</span></span>|
|<span data-ttu-id="ab58a-151">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="ab58a-151">managedGroupTypes</span></span>|<span data-ttu-id="ab58a-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab58a-152">String</span></span>| <span data-ttu-id="ab58a-153">O tipo de grupo ao qual se aplica a política de expiração.</span><span class="sxs-lookup"><span data-stu-id="ab58a-153">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="ab58a-154">Os valores possíveis são **All**, **Selected** ou **None**.</span><span class="sxs-lookup"><span data-stu-id="ab58a-154">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ab58a-155">Relações</span><span class="sxs-lookup"><span data-stu-id="ab58a-155">Relationships</span></span>

<span data-ttu-id="ab58a-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab58a-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab58a-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab58a-157">JSON representation</span></span>

<span data-ttu-id="ab58a-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab58a-158">Here is a JSON representation of the resource.</span></span>

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

