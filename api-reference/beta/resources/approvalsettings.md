---
title: tipo complexo approvalSettings
description: Usado para a propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e248e47cf94e2c26e80b505cbaead450e03561d4
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331358"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="d19c4-104">tipo complexo approvalSettings</span><span class="sxs-lookup"><span data-stu-id="d19c4-104">approvalSettings complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d19c4-105">Usada para a `requestApprovalSettings` propriedade de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d19c4-105">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="d19c4-106">Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.</span><span class="sxs-lookup"><span data-stu-id="d19c4-106">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="d19c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d19c4-107">Properties</span></span>

| <span data-ttu-id="d19c4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d19c4-108">Property</span></span>                     | <span data-ttu-id="d19c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d19c4-109">Type</span></span>                      | <span data-ttu-id="d19c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d19c4-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d19c4-111">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="d19c4-111">isApprovalRequired</span></span> | <span data-ttu-id="d19c4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="d19c4-112">Boolean</span></span> | <span data-ttu-id="d19c4-113">Se for false, a aprovação não será necessária para solicitações nesta política.</span><span class="sxs-lookup"><span data-stu-id="d19c4-113">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="d19c4-114">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="d19c4-114">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="d19c4-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="d19c4-115">Boolean</span></span>| <span data-ttu-id="d19c4-116">Se for false, a aprovação não será necessária para um usuário que já tenha uma atribuição para estender sua atribuição.</span><span class="sxs-lookup"><span data-stu-id="d19c4-116">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="d19c4-117">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="d19c4-117">isRequestorJustificationRequired</span></span> | <span data-ttu-id="d19c4-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="d19c4-118">Boolean</span></span> | <span data-ttu-id="d19c4-119">Indica se o solicitante é necessário para fornecer uma justificativa em sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="d19c4-119">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="d19c4-120">approvalmode</span><span class="sxs-lookup"><span data-stu-id="d19c4-120">approvalMode</span></span>| <span data-ttu-id="d19c4-121">String</span><span class="sxs-lookup"><span data-stu-id="d19c4-121">String</span></span> | <span data-ttu-id="d19c4-122">Um de `NoApproval`, `SingleStage` ou `Serial`.</span><span class="sxs-lookup"><span data-stu-id="d19c4-122">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="d19c4-123">O `NoApproval` é usado quando `isApprovalRequired` é falso.</span><span class="sxs-lookup"><span data-stu-id="d19c4-123">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="d19c4-124">approvalStages</span><span class="sxs-lookup"><span data-stu-id="d19c4-124">approvalStages</span></span> | <span data-ttu-id="d19c4-125">coleção [approvalStage](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="d19c4-125">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="d19c4-126">Se for necessário aprovar, um ou dois elementos dessa coleção define cada um dos estágios de aprovação.</span><span class="sxs-lookup"><span data-stu-id="d19c4-126">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="d19c4-127">Uma matriz vazia se nenhuma aprovação for necessária.</span><span class="sxs-lookup"><span data-stu-id="d19c4-127">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d19c4-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d19c4-128">JSON representation</span></span>

<span data-ttu-id="d19c4-129">Veja a seguir uma representação JSON da propriedade solicitar configurações de aprovação.</span><span class="sxs-lookup"><span data-stu-id="d19c4-129">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
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
