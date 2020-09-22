---
title: tipo complexo approvalStage
description: Usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df7e9ce4491ea7a887b79f79d354c9099ea9f5d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050138"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="70718-104">tipo complexo approvalStage</span><span class="sxs-lookup"><span data-stu-id="70718-104">approvalStage complex type</span></span>

<span data-ttu-id="70718-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70718-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70718-106">Usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="70718-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="70718-107">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="70718-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="70718-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70718-108">Properties</span></span>

| <span data-ttu-id="70718-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70718-109">Property</span></span>                     | <span data-ttu-id="70718-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="70718-110">Type</span></span>                      | <span data-ttu-id="70718-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="70718-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="70718-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="70718-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="70718-113">Int32</span><span class="sxs-lookup"><span data-stu-id="70718-113">Int32</span></span> | <span data-ttu-id="70718-114">O número de dias que uma solicitação pode aguardar uma resposta antes de ser automaticamente negada.</span><span class="sxs-lookup"><span data-stu-id="70718-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="70718-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="70718-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="70718-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="70718-116">Boolean</span></span> | <span data-ttu-id="70718-117">Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="70718-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="70718-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="70718-118">isEscalationEnabled</span></span> |<span data-ttu-id="70718-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="70718-119">Boolean</span></span> | <span data-ttu-id="70718-120">Se true, um ou mais aprovadores de escalonamento estão configurados neste estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="70718-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="70718-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="70718-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="70718-122">Int32</span><span class="sxs-lookup"><span data-stu-id="70718-122">Int32</span></span> | <span data-ttu-id="70718-123">Se for necessário escalonamento, o tempo em que uma solicitação pode ser pendente é uma resposta de um Aprovador principal.</span><span class="sxs-lookup"><span data-stu-id="70718-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="70718-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="70718-124">primaryApprovers</span></span> | <span data-ttu-id="70718-125">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="70718-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="70718-126">Os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="70718-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="70718-127">Uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="70718-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="70718-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="70718-128">escalationApprovers</span></span> | <span data-ttu-id="70718-129">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="70718-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="70718-130">Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers são os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="70718-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="70718-131">Pode ser uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="70718-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="70718-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70718-132">JSON representation</span></span>

<span data-ttu-id="70718-133">Veja a seguir uma representação JSON da fase solicitar aprovação.</span><span class="sxs-lookup"><span data-stu-id="70718-133">The following is a JSON representation of the request approval stage.</span></span>

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


