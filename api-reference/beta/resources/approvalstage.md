---
title: tipo complexo approvalStage
description: Usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a478f7b0ed06a247ece20ac14763f7de8ff498d
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331346"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="df917-104">tipo complexo approvalStage</span><span class="sxs-lookup"><span data-stu-id="df917-104">approvalStage complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df917-105">Usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="df917-105">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="df917-106">Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.</span><span class="sxs-lookup"><span data-stu-id="df917-106">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="df917-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df917-107">Properties</span></span>

| <span data-ttu-id="df917-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df917-108">Property</span></span>                     | <span data-ttu-id="df917-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df917-109">Type</span></span>                      | <span data-ttu-id="df917-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df917-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="df917-111">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="df917-111">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="df917-112">Int32</span><span class="sxs-lookup"><span data-stu-id="df917-112">Int32</span></span> | <span data-ttu-id="df917-113">O número de dias que uma solicitação pode aguardar uma resposta antes de ser automaticamente negada.</span><span class="sxs-lookup"><span data-stu-id="df917-113">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="df917-114">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="df917-114">isApproverJustificationRequired</span></span> |<span data-ttu-id="df917-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="df917-115">Boolean</span></span> | <span data-ttu-id="df917-116">Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="df917-116">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="df917-117">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="df917-117">isEscalationEnabled</span></span> |<span data-ttu-id="df917-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="df917-118">Boolean</span></span> | <span data-ttu-id="df917-119">Se true, um ou mais aprovadores de escalonamento estão configurados neste estágio de aprovação.</span><span class="sxs-lookup"><span data-stu-id="df917-119">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="df917-120">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="df917-120">escalationTimeInMinutes</span></span> |<span data-ttu-id="df917-121">Int32</span><span class="sxs-lookup"><span data-stu-id="df917-121">Int32</span></span> | <span data-ttu-id="df917-122">Se for necessário escalonamento, o tempo em que uma solicitação pode ser pendente é uma resposta de um Aprovador principal.</span><span class="sxs-lookup"><span data-stu-id="df917-122">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="df917-123">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="df917-123">primaryApprovers</span></span> | <span data-ttu-id="df917-124">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="df917-124">[userSet](userset.md) collection</span></span>| <span data-ttu-id="df917-125">Os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="df917-125">The users who will be asked to approve requests.</span></span> <span data-ttu-id="df917-126">Uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="df917-126">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="df917-127">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="df917-127">escalationApprovers</span></span> | <span data-ttu-id="df917-128">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="df917-128">[userSet](userset.md) collection</span></span>| <span data-ttu-id="df917-129">Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers são os usuários que serão solicitados a aprovar solicitações.</span><span class="sxs-lookup"><span data-stu-id="df917-129">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="df917-130">Pode ser uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).</span><span class="sxs-lookup"><span data-stu-id="df917-130">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="df917-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df917-131">JSON representation</span></span>

<span data-ttu-id="df917-132">Veja a seguir uma representação JSON da fase solicitar aprovação.</span><span class="sxs-lookup"><span data-stu-id="df917-132">The following is a JSON representation of the request approval stage.</span></span>

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
