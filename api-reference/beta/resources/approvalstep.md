---
title: Tipo de recurso approvalStep
description: O objeto approvalStep associado ao accessPackageAssignmentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 263e809e5858cdc23b34b8401171bb5fce668721
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761251"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="20a58-103">Tipo de recurso approvalStep</span><span class="sxs-lookup"><span data-stu-id="20a58-103">approvalStep resource type</span></span>

<span data-ttu-id="20a58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20a58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20a58-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto approvalStep para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="20a58-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="20a58-106">Ele é usado para distinguir decisões para diferentes etapas de um fluxo de trabalho de aprovação em que os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="20a58-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

## <a name="methods"></a><span data-ttu-id="20a58-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="20a58-107">Methods</span></span>

| <span data-ttu-id="20a58-108">Método</span><span class="sxs-lookup"><span data-stu-id="20a58-108">Method</span></span>       | <span data-ttu-id="20a58-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20a58-109">Return Type</span></span> | <span data-ttu-id="20a58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a58-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="20a58-111">Aprovação de listaSteps</span><span class="sxs-lookup"><span data-stu-id="20a58-111">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="20a58-112">[Coleção approvalStep](approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="20a58-112">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="20a58-113">Listar **os objetos approvalStep** associados a um **objeto de** aprovação.</span><span class="sxs-lookup"><span data-stu-id="20a58-113">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="20a58-114">Obter approvalStep</span><span class="sxs-lookup"><span data-stu-id="20a58-114">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="20a58-115">approvalStep</span><span class="sxs-lookup"><span data-stu-id="20a58-115">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="20a58-116">Recupere as propriedades de um **objeto approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="20a58-116">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="20a58-117">Atualizar approvalStep</span><span class="sxs-lookup"><span data-stu-id="20a58-117">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="20a58-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20a58-118">None</span></span> | <span data-ttu-id="20a58-119">Aplicar aprovar ou negar decisão em um **objeto approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="20a58-119">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="20a58-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20a58-120">Properties</span></span>
|<span data-ttu-id="20a58-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20a58-121">Property</span></span>|<span data-ttu-id="20a58-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="20a58-122">Type</span></span>|<span data-ttu-id="20a58-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a58-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20a58-124">id</span><span class="sxs-lookup"><span data-stu-id="20a58-124">id</span></span>|<span data-ttu-id="20a58-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20a58-125">String</span></span>|<span data-ttu-id="20a58-126">O identificador da etapa associada a um objeto de aprovação.</span><span class="sxs-lookup"><span data-stu-id="20a58-126">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="20a58-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20a58-127">Read-only.</span></span>|
|<span data-ttu-id="20a58-128">displayName</span><span class="sxs-lookup"><span data-stu-id="20a58-128">displayName</span></span>|<span data-ttu-id="20a58-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20a58-129">String</span></span>|<span data-ttu-id="20a58-130">O rótulo fornecido pelo criador da política para identificar uma etapa de aprovação.</span><span class="sxs-lookup"><span data-stu-id="20a58-130">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="20a58-131">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="20a58-131">Read-only</span></span>|
|<span data-ttu-id="20a58-132">status</span><span class="sxs-lookup"><span data-stu-id="20a58-132">status</span></span>|<span data-ttu-id="20a58-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20a58-133">String</span></span>|<span data-ttu-id="20a58-134">O status da etapa.</span><span class="sxs-lookup"><span data-stu-id="20a58-134">The step status.</span></span> <span data-ttu-id="20a58-135">Valores possíveis: `InProgress` ou `Completed` .</span><span class="sxs-lookup"><span data-stu-id="20a58-135">Possible values: `InProgress` or `Completed`.</span></span> <span data-ttu-id="20a58-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20a58-136">Read-only.</span></span>|
|<span data-ttu-id="20a58-137">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="20a58-137">assignedToMe</span></span>|<span data-ttu-id="20a58-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="20a58-138">Boolean</span></span>|<span data-ttu-id="20a58-139">Indica se a etapa é atribuída ao usuário chamador para revisar.</span><span class="sxs-lookup"><span data-stu-id="20a58-139">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="20a58-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20a58-140">Read-only.</span></span>|
|<span data-ttu-id="20a58-141">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="20a58-141">reviewedBy</span></span>|<span data-ttu-id="20a58-142">[Coleção userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="20a58-142">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="20a58-143">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="20a58-143">The identifier of the reviewer.</span></span> <span data-ttu-id="20a58-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20a58-144">Read-only.</span></span>|
|<span data-ttu-id="20a58-145">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="20a58-145">reviewedDateTime</span></span>|<span data-ttu-id="20a58-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20a58-146">DateTimeOffset</span></span>|<span data-ttu-id="20a58-147">A data e a hora em que uma decisão foi registrada.</span><span class="sxs-lookup"><span data-stu-id="20a58-147">The date and time when a decision was recorded.</span></span> <span data-ttu-id="20a58-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20a58-148">Read-only.</span></span>|
|<span data-ttu-id="20a58-149">reviewResult</span><span class="sxs-lookup"><span data-stu-id="20a58-149">reviewResult</span></span>|<span data-ttu-id="20a58-150">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="20a58-150">String</span></span>|<span data-ttu-id="20a58-151">O resultado desse registro de aprovação.</span><span class="sxs-lookup"><span data-stu-id="20a58-151">The result of this approval record.</span></span> <span data-ttu-id="20a58-152">Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="20a58-152">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="20a58-153">justification</span><span class="sxs-lookup"><span data-stu-id="20a58-153">justification</span></span>|<span data-ttu-id="20a58-154">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="20a58-154">String</span></span>|<span data-ttu-id="20a58-155">A justificativa associada à decisão da etapa de aprovação.</span><span class="sxs-lookup"><span data-stu-id="20a58-155">The justification associated with the approval step decision.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20a58-156">Relações</span><span class="sxs-lookup"><span data-stu-id="20a58-156">Relationships</span></span>
|<span data-ttu-id="20a58-157">Relação</span><span class="sxs-lookup"><span data-stu-id="20a58-157">Relationship</span></span>|<span data-ttu-id="20a58-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="20a58-158">Type</span></span>|<span data-ttu-id="20a58-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a58-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20a58-160">aprovação</span><span class="sxs-lookup"><span data-stu-id="20a58-160">approval</span></span>|<span data-ttu-id="20a58-161">[coleção approval](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="20a58-161">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="20a58-162">O objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="20a58-162">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20a58-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20a58-163">JSON representation</span></span>
<span data-ttu-id="20a58-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20a58-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalStep",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": true,
  "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String",
}
```
