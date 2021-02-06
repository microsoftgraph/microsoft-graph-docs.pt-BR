---
title: tipo complexo approvalStage
description: Usada para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma diretiva de atribuição de pacote de acesso. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d24f8def3520cf2605f30dc47ab06f52e09fc163
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135251"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="18e6d-104">tipo complexo approvalStage</span><span class="sxs-lookup"><span data-stu-id="18e6d-104">approvalStage complex type</span></span>

<span data-ttu-id="18e6d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18e6d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e6d-106">Usado para a **propriedade approvalStages** das configurações de aprovação na **propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="18e6d-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="18e6d-107">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="18e6d-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="18e6d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18e6d-108">Properties</span></span>

| <span data-ttu-id="18e6d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18e6d-109">Property</span></span>                     | <span data-ttu-id="18e6d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18e6d-110">Type</span></span>                      | <span data-ttu-id="18e6d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18e6d-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="18e6d-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="18e6d-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="18e6d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="18e6d-113">Int32</span></span> | <span data-ttu-id="18e6d-114">O número de dias que uma solicitação pode estar aguardando uma resposta antes de ser negada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="18e6d-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="18e6d-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="18e6d-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="18e6d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="18e6d-116">Boolean</span></span> | <span data-ttu-id="18e6d-117">Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="18e6d-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="18e6d-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="18e6d-118">isEscalationEnabled</span></span> |<span data-ttu-id="18e6d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="18e6d-119">Boolean</span></span> | <span data-ttu-id="18e6d-120">Se for verdadeiro, um ou mais aprovadores de escalonamento serão configurados nesse estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="18e6d-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="18e6d-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="18e6d-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="18e6d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="18e6d-122">Int32</span></span> | <span data-ttu-id="18e6d-123">Se o escalonamento for necessário, o tempo em que uma solicitação poderá estar aguardando uma resposta de um aprovador primário.</span><span class="sxs-lookup"><span data-stu-id="18e6d-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="18e6d-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="18e6d-124">primaryApprovers</span></span> | <span data-ttu-id="18e6d-125">[Coleção userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="18e6d-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="18e6d-126">Os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="18e6d-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="18e6d-127">Uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="18e6d-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="18e6d-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="18e6d-128">escalationApprovers</span></span> | <span data-ttu-id="18e6d-129">[Coleção userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="18e6d-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="18e6d-130">Se o escalonamento estiver habilitado e os aprovadores principais não responderem antes do tempo de escalonamento, os escalationApprovers serão os usuários que serão solicitados a aprovar as solicitações.</span><span class="sxs-lookup"><span data-stu-id="18e6d-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="18e6d-131">Pode ser uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="18e6d-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="18e6d-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18e6d-132">JSON representation</span></span>

<span data-ttu-id="18e6d-133">A seguir está uma representação JSON do estágio de aprovação de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18e6d-133">The following is a JSON representation of the request approval stage.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage"
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


