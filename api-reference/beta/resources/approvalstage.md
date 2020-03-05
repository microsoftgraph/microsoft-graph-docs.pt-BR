---
title: tipo complexo approvalStage
description: Usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0edcb4af5ae6bbc154d0748b57ec83efcb3137f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508223"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="5eb3e-104">tipo complexo approvalStage</span><span class="sxs-lookup"><span data-stu-id="5eb3e-104">approvalStage complex type</span></span>

<span data-ttu-id="5eb3e-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5eb3e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eb3e-106">Usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5eb3e-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="5eb3e-107">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="5eb3e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5eb3e-108">Properties</span></span>

| <span data-ttu-id="5eb3e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5eb3e-109">Property</span></span>                     | <span data-ttu-id="5eb3e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5eb3e-110">Type</span></span>                      | <span data-ttu-id="5eb3e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5eb3e-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="5eb3e-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="5eb3e-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="5eb3e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5eb3e-113">Int32</span></span> | <span data-ttu-id="5eb3e-114">O número de dias que uma solicitação pode aguardar uma resposta antes de ser automaticamente negada.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="5eb3e-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="5eb3e-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="5eb3e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eb3e-116">Boolean</span></span> | <span data-ttu-id="5eb3e-117">Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="5eb3e-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="5eb3e-118">isEscalationEnabled</span></span> |<span data-ttu-id="5eb3e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5eb3e-119">Boolean</span></span> | <span data-ttu-id="5eb3e-120">Se true, um ou mais aprovadores de escalonamento estão configurados neste estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="5eb3e-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="5eb3e-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="5eb3e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5eb3e-122">Int32</span></span> | <span data-ttu-id="5eb3e-123">Se for necessário escalonamento, o tempo em que uma solicitação pode ser pendente é uma resposta de um Aprovador principal.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="5eb3e-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="5eb3e-124">primaryApprovers</span></span> | <span data-ttu-id="5eb3e-125">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="5eb3e-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="5eb3e-126">Os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="5eb3e-127">Uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="5eb3e-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="5eb3e-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="5eb3e-128">escalationApprovers</span></span> | <span data-ttu-id="5eb3e-129">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="5eb3e-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="5eb3e-130">Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers são os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="5eb3e-131">Pode ser uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="5eb3e-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="5eb3e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5eb3e-132">JSON representation</span></span>

<span data-ttu-id="5eb3e-133">Veja a seguir uma representação JSON da fase solicitar aprovação.</span><span class="sxs-lookup"><span data-stu-id="5eb3e-133">The following is a JSON representation of the request approval stage.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage",
  "baseType": ""
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
