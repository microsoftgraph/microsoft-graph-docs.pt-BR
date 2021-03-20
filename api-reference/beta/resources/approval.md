---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um accessPackageAssignmentRequest ou userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f6751807f0dcb042958104c4b3146a555b22189
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945715"
---
# <a name="approval-resource-type"></a><span data-ttu-id="f5da6-103">tipo de recurso de aprovação</span><span class="sxs-lookup"><span data-stu-id="f5da6-103">approval resource type</span></span>

<span data-ttu-id="f5da6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5da6-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="f5da6-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="f5da6-106">Uma única solicitação de etapa pode ter uma etapa associada a ela na qual os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="f5da6-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="f5da6-107">Da mesma forma, uma solicitação em várias etapas pode ter várias etapas associadas a ela nas quais os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="f5da6-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="f5da6-108">No entanto, em aprovações em várias etapas, as etapas pendentes e concluídas anteriormente são mostradas.</span><span class="sxs-lookup"><span data-stu-id="f5da6-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

<span data-ttu-id="f5da6-109">Em [userConsentRequests](../resources/userconsentrequest.md), o objeto de aprovação para decisões associadas a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5da6-109">In [userConsentRequests](../resources/userconsentrequest.md), the approval object for decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="f5da6-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f5da6-110">Methods</span></span>

| <span data-ttu-id="f5da6-111">Método</span><span class="sxs-lookup"><span data-stu-id="f5da6-111">Method</span></span>       | <span data-ttu-id="f5da6-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f5da6-112">Return Type</span></span> | <span data-ttu-id="f5da6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5da6-113">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="f5da6-114">Obter aprovação</span><span class="sxs-lookup"><span data-stu-id="f5da6-114">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="f5da6-115">aprovação</span><span class="sxs-lookup"><span data-stu-id="f5da6-115">approval</span></span>](approval.md) | <span data-ttu-id="f5da6-116">Recupere as propriedades de um **objeto de aprovação.**</span><span class="sxs-lookup"><span data-stu-id="f5da6-116">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="f5da6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5da6-117">Properties</span></span>
|<span data-ttu-id="f5da6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5da6-118">Property</span></span>|<span data-ttu-id="f5da6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5da6-119">Type</span></span>|<span data-ttu-id="f5da6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5da6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5da6-121">id</span><span class="sxs-lookup"><span data-stu-id="f5da6-121">id</span></span>|<span data-ttu-id="f5da6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5da6-122">String</span></span>|<span data-ttu-id="f5da6-123">O identificador do objeto de aprovação.</span><span class="sxs-lookup"><span data-stu-id="f5da6-123">The identifier of the approval object.</span></span>|
|<span data-ttu-id="f5da6-124">etapas</span><span class="sxs-lookup"><span data-stu-id="f5da6-124">steps</span></span>|<span data-ttu-id="f5da6-125">[Coleção approvalStep](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="f5da6-125">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="f5da6-126">Usado para representar a decisão associada a uma única etapa no processo de aprovação configurado em [approvalStage](../resources/approvalstage.md).</span><span class="sxs-lookup"><span data-stu-id="f5da6-126">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5da6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f5da6-127">Relationships</span></span>
|<span data-ttu-id="f5da6-128">Relação</span><span class="sxs-lookup"><span data-stu-id="f5da6-128">Relationship</span></span>|<span data-ttu-id="f5da6-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5da6-129">Type</span></span>|<span data-ttu-id="f5da6-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5da6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5da6-131">Estágios</span><span class="sxs-lookup"><span data-stu-id="f5da6-131">stages</span></span>|<span data-ttu-id="f5da6-132">[coleção approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="f5da6-132">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="f5da6-133">Usada para a **propriedade approvalStages** das configurações de aprovação **na propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f5da6-133">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="f5da6-134">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="f5da6-134">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f5da6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5da6-135">JSON representation</span></span>
<span data-ttu-id="f5da6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5da6-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
