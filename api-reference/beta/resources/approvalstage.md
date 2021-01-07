---
title: tipo complexo approvalStage
description: Usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 158fae1675c26876daeb05b1571d7fd91855df72
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777698"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="71aba-104">tipo complexo approvalStage</span><span class="sxs-lookup"><span data-stu-id="71aba-104">approvalStage complex type</span></span>

<span data-ttu-id="71aba-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71aba-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71aba-106">Usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71aba-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="71aba-107">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="71aba-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="71aba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71aba-108">Properties</span></span>

| <span data-ttu-id="71aba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71aba-109">Property</span></span>                     | <span data-ttu-id="71aba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="71aba-110">Type</span></span>                      | <span data-ttu-id="71aba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71aba-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="71aba-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="71aba-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="71aba-113">Int32</span><span class="sxs-lookup"><span data-stu-id="71aba-113">Int32</span></span> | <span data-ttu-id="71aba-114">O número de dias que uma solicitação pode aguardar uma resposta antes de ser automaticamente negada.</span><span class="sxs-lookup"><span data-stu-id="71aba-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="71aba-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="71aba-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="71aba-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="71aba-116">Boolean</span></span> | <span data-ttu-id="71aba-117">Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="71aba-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="71aba-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="71aba-118">isEscalationEnabled</span></span> |<span data-ttu-id="71aba-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="71aba-119">Boolean</span></span> | <span data-ttu-id="71aba-120">Se true, um ou mais aprovadores de escalonamento estão configurados neste estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="71aba-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="71aba-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="71aba-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="71aba-122">Int32</span><span class="sxs-lookup"><span data-stu-id="71aba-122">Int32</span></span> | <span data-ttu-id="71aba-123">Se for necessário escalonamento, o tempo em que uma solicitação pode ser pendente é uma resposta de um Aprovador principal.</span><span class="sxs-lookup"><span data-stu-id="71aba-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="71aba-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="71aba-124">primaryApprovers</span></span> | <span data-ttu-id="71aba-125">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="71aba-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="71aba-126">Os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="71aba-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="71aba-127">Uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="71aba-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="71aba-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="71aba-128">escalationApprovers</span></span> | <span data-ttu-id="71aba-129">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="71aba-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="71aba-130">Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers são os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="71aba-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="71aba-131">Pode ser uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="71aba-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="71aba-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71aba-132">JSON representation</span></span>

<span data-ttu-id="71aba-133">Veja a seguir uma representação JSON da fase solicitar aprovação.</span><span class="sxs-lookup"><span data-stu-id="71aba-133">The following is a JSON representation of the request approval stage.</span></span>

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


