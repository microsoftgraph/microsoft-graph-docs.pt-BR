---
title: Tipo de recurso approvalStep
description: O objeto approvalStep associado a um accessPackageAssignmentRequest ou userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 413af698c72be945e648a3fe21ce772f2b4e6102
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061872"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="1a165-103">Tipo de recurso approvalStep</span><span class="sxs-lookup"><span data-stu-id="1a165-103">approvalStep resource type</span></span>

<span data-ttu-id="1a165-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a165-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto approvalStep para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="1a165-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="1a165-106">Ele é usado para distinguir decisões para diferentes etapas de um fluxo de trabalho de aprovação em que os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="1a165-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

<span data-ttu-id="1a165-107">Em [userConsentRequests](../resources/userconsentrequest.md), as decisões de aprovação associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a165-107">In [userConsentRequests](../resources/userconsentrequest.md), the approval  decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="1a165-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a165-108">Methods</span></span>

| <span data-ttu-id="1a165-109">Método</span><span class="sxs-lookup"><span data-stu-id="1a165-109">Method</span></span>       | <span data-ttu-id="1a165-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a165-110">Return Type</span></span> | <span data-ttu-id="1a165-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a165-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="1a165-112">Aprovação de listaSteps</span><span class="sxs-lookup"><span data-stu-id="1a165-112">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="1a165-113">[Coleção approvalStep](approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="1a165-113">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="1a165-114">Listar **os objetos approvalStep** associados a um **objeto de** aprovação.</span><span class="sxs-lookup"><span data-stu-id="1a165-114">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="1a165-115">Obter approvalStep</span><span class="sxs-lookup"><span data-stu-id="1a165-115">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="1a165-116">approvalStep</span><span class="sxs-lookup"><span data-stu-id="1a165-116">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="1a165-117">Recupere as propriedades de um **objeto approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="1a165-117">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="1a165-118">Atualizar approvalStep</span><span class="sxs-lookup"><span data-stu-id="1a165-118">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="1a165-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a165-119">None</span></span> | <span data-ttu-id="1a165-120">Aplicar aprovar ou negar decisão em um **objeto approvalStep.**</span><span class="sxs-lookup"><span data-stu-id="1a165-120">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a165-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a165-121">Properties</span></span>
|<span data-ttu-id="1a165-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a165-122">Property</span></span>|<span data-ttu-id="1a165-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a165-123">Type</span></span>|<span data-ttu-id="1a165-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a165-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a165-125">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="1a165-125">assignedToMe</span></span>|<span data-ttu-id="1a165-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a165-126">Boolean</span></span>|<span data-ttu-id="1a165-127">Indica se a etapa é atribuída ao usuário chamador para revisar.</span><span class="sxs-lookup"><span data-stu-id="1a165-127">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="1a165-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-128">Read-only.</span></span>|
|<span data-ttu-id="1a165-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1a165-129">displayName</span></span>|<span data-ttu-id="1a165-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a165-130">String</span></span>|<span data-ttu-id="1a165-131">O rótulo fornecido pelo criador da política para identificar uma etapa de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1a165-131">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="1a165-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-132">Read-only.</span></span>|
|<span data-ttu-id="1a165-133">id</span><span class="sxs-lookup"><span data-stu-id="1a165-133">id</span></span>|<span data-ttu-id="1a165-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a165-134">String</span></span>|<span data-ttu-id="1a165-135">O identificador da etapa associada a um objeto de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1a165-135">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="1a165-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-136">Read-only.</span></span>|
|<span data-ttu-id="1a165-137">justification</span><span class="sxs-lookup"><span data-stu-id="1a165-137">justification</span></span>|<span data-ttu-id="1a165-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a165-138">String</span></span>|<span data-ttu-id="1a165-139">A justificativa associada à decisão da etapa de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1a165-139">The justification associated with the approval step decision.</span></span>|
|<span data-ttu-id="1a165-140">reviewResult</span><span class="sxs-lookup"><span data-stu-id="1a165-140">reviewResult</span></span>|<span data-ttu-id="1a165-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a165-141">String</span></span>|<span data-ttu-id="1a165-142">O resultado desse registro de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1a165-142">The result of this approval record.</span></span> <span data-ttu-id="1a165-143">Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .</span><span class="sxs-lookup"><span data-stu-id="1a165-143">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="1a165-144">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="1a165-144">reviewedBy</span></span>|<span data-ttu-id="1a165-145">[Coleção userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="1a165-145">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="1a165-146">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="1a165-146">The identifier of the reviewer.</span></span> <span data-ttu-id="1a165-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-147">Read-only.</span></span>|
|<span data-ttu-id="1a165-148">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a165-148">reviewedDateTime</span></span>|<span data-ttu-id="1a165-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a165-149">DateTimeOffset</span></span>|<span data-ttu-id="1a165-150">A data e a hora em que uma decisão foi registrada.</span><span class="sxs-lookup"><span data-stu-id="1a165-150">The date and time when a decision was recorded.</span></span> <span data-ttu-id="1a165-151">As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1a165-151">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1a165-152">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1a165-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1a165-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-153">Read-only.</span></span>|
|<span data-ttu-id="1a165-154">status</span><span class="sxs-lookup"><span data-stu-id="1a165-154">status</span></span>|<span data-ttu-id="1a165-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a165-155">String</span></span>|<span data-ttu-id="1a165-156">O status da etapa.</span><span class="sxs-lookup"><span data-stu-id="1a165-156">The step status.</span></span> <span data-ttu-id="1a165-157">Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` .</span><span class="sxs-lookup"><span data-stu-id="1a165-157">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="1a165-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a165-158">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1a165-159">Relações</span><span class="sxs-lookup"><span data-stu-id="1a165-159">Relationships</span></span>
|<span data-ttu-id="1a165-160">Relação</span><span class="sxs-lookup"><span data-stu-id="1a165-160">Relationship</span></span>|<span data-ttu-id="1a165-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a165-161">Type</span></span>|<span data-ttu-id="1a165-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a165-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a165-163">aprovação</span><span class="sxs-lookup"><span data-stu-id="1a165-163">approval</span></span>|<span data-ttu-id="1a165-164">[coleção approval](../resources/approval.md)</span><span class="sxs-lookup"><span data-stu-id="1a165-164">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="1a165-165">O objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="1a165-165">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a165-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a165-166">JSON representation</span></span>
<span data-ttu-id="1a165-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a165-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
   "@odata.type":"#microsoft.graph.approvalStep",
   "id":"String (identifier)",
   "displayName":"String",
   "status":"String",
   "assignedToMe":true,
   "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
   "reviewedDateTime":"String (timestamp)",
   "reviewResult":"String",
   "justification":"String"
}
```
