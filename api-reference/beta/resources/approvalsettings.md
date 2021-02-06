---
title: Tipo complexo approvalSettings
description: Usada para a propriedade requestApprovalSettings de uma diretiva de atribuição de pacote de acesso. Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99892e0943b993fe43edb4bd104fd2a3a8736a51
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135252"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="7646d-104">Tipo complexo approvalSettings</span><span class="sxs-lookup"><span data-stu-id="7646d-104">approvalSettings complex type</span></span>

<span data-ttu-id="7646d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7646d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7646d-106">Usado para a propriedade `requestApprovalSettings` de uma política de [atribuição de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7646d-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="7646d-107">Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.</span><span class="sxs-lookup"><span data-stu-id="7646d-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="7646d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7646d-108">Properties</span></span>

| <span data-ttu-id="7646d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7646d-109">Property</span></span>                     | <span data-ttu-id="7646d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7646d-110">Type</span></span>                      | <span data-ttu-id="7646d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7646d-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="7646d-112">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="7646d-112">isApprovalRequired</span></span> | <span data-ttu-id="7646d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="7646d-113">Boolean</span></span> | <span data-ttu-id="7646d-114">Se for falso, a aprovação não será necessária para solicitações nesta política.</span><span class="sxs-lookup"><span data-stu-id="7646d-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="7646d-115">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="7646d-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="7646d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7646d-116">Boolean</span></span>| <span data-ttu-id="7646d-117">Se for falso, a aprovação não será necessária para um usuário que já tenha uma atribuição para estender sua atribuição.</span><span class="sxs-lookup"><span data-stu-id="7646d-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="7646d-118">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="7646d-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="7646d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7646d-119">Boolean</span></span> | <span data-ttu-id="7646d-120">Indica se o solicitante é obrigado a fornecer uma justificativa em sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="7646d-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="7646d-121">approvalMode</span><span class="sxs-lookup"><span data-stu-id="7646d-121">approvalMode</span></span>| <span data-ttu-id="7646d-122">String</span><span class="sxs-lookup"><span data-stu-id="7646d-122">String</span></span> | <span data-ttu-id="7646d-123">Um dos `NoApproval` , `SingleStage` ou `Serial` .</span><span class="sxs-lookup"><span data-stu-id="7646d-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="7646d-124">O `NoApproval` é usado quando é `isApprovalRequired` falso.</span><span class="sxs-lookup"><span data-stu-id="7646d-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="7646d-125">approvalStages</span><span class="sxs-lookup"><span data-stu-id="7646d-125">approvalStages</span></span> | <span data-ttu-id="7646d-126">[coleção approvalStage](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="7646d-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="7646d-127">Se a aprovação for necessária, um ou dois elementos dessa coleção definirão cada um dos estágios de aprovação.</span><span class="sxs-lookup"><span data-stu-id="7646d-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="7646d-128">Uma matriz vazia se nenhuma aprovação for necessária.</span><span class="sxs-lookup"><span data-stu-id="7646d-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7646d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7646d-129">JSON representation</span></span>

<span data-ttu-id="7646d-130">A seguir está uma representação JSON da propriedade de configurações de aprovação de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7646d-130">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
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


