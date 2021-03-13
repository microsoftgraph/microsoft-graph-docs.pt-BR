---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado ao accessPackageAssignmentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d46630b563674153ef687a8e8f86dce70eec9985
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761258"
---
# <a name="approval-resource-type"></a><span data-ttu-id="7d030-103">tipo de recurso de aprovação</span><span class="sxs-lookup"><span data-stu-id="7d030-103">approval resource type</span></span>

<span data-ttu-id="7d030-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d030-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d030-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` .</span><span class="sxs-lookup"><span data-stu-id="7d030-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="7d030-106">Uma única solicitação de etapa pode ter uma etapa associada a ela na qual os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="7d030-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="7d030-107">Da mesma forma, uma solicitação em várias etapas pode ter várias etapas associadas a ela nas quais os aprovadores podem agir.</span><span class="sxs-lookup"><span data-stu-id="7d030-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="7d030-108">No entanto, em aprovações em várias etapas, as etapas pendentes e concluídas anteriormente são mostradas.</span><span class="sxs-lookup"><span data-stu-id="7d030-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

## <a name="methods"></a><span data-ttu-id="7d030-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d030-109">Methods</span></span>

| <span data-ttu-id="7d030-110">Método</span><span class="sxs-lookup"><span data-stu-id="7d030-110">Method</span></span>       | <span data-ttu-id="7d030-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d030-111">Return Type</span></span> | <span data-ttu-id="7d030-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d030-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="7d030-113">Obter aprovação</span><span class="sxs-lookup"><span data-stu-id="7d030-113">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="7d030-114">aprovação</span><span class="sxs-lookup"><span data-stu-id="7d030-114">approval</span></span>](approval.md) | <span data-ttu-id="7d030-115">Recupere as propriedades de um **objeto de aprovação.**</span><span class="sxs-lookup"><span data-stu-id="7d030-115">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="7d030-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d030-116">Properties</span></span>
|<span data-ttu-id="7d030-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d030-117">Property</span></span>|<span data-ttu-id="7d030-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d030-118">Type</span></span>|<span data-ttu-id="7d030-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d030-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d030-120">id</span><span class="sxs-lookup"><span data-stu-id="7d030-120">id</span></span>|<span data-ttu-id="7d030-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d030-121">String</span></span>|<span data-ttu-id="7d030-122">O identificador do objeto de aprovação.</span><span class="sxs-lookup"><span data-stu-id="7d030-122">The identifier of the approval object.</span></span>|
|<span data-ttu-id="7d030-123">etapas</span><span class="sxs-lookup"><span data-stu-id="7d030-123">steps</span></span>|<span data-ttu-id="7d030-124">[Coleção approvalStep](../resources/approvalstep.md)</span><span class="sxs-lookup"><span data-stu-id="7d030-124">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="7d030-125">Usado para representar a decisão associada a uma única etapa no processo de aprovação configurado em [approvalStage](../resources/approvalstage.md).</span><span class="sxs-lookup"><span data-stu-id="7d030-125">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d030-126">Relações</span><span class="sxs-lookup"><span data-stu-id="7d030-126">Relationships</span></span>
|<span data-ttu-id="7d030-127">Relação</span><span class="sxs-lookup"><span data-stu-id="7d030-127">Relationship</span></span>|<span data-ttu-id="7d030-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d030-128">Type</span></span>|<span data-ttu-id="7d030-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d030-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d030-130">Estágios</span><span class="sxs-lookup"><span data-stu-id="7d030-130">stages</span></span>|<span data-ttu-id="7d030-131">[coleção approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="7d030-131">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="7d030-132">Usada para a **propriedade approvalStages** das configurações de aprovação **na propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7d030-132">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="7d030-133">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="7d030-133">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7d030-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d030-134">JSON representation</span></span>
<span data-ttu-id="7d030-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d030-135">The following is a JSON representation of the resource.</span></span>
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
