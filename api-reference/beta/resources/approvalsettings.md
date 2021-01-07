---
title: tipo complexo approvalSettings
description: Usado para a propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85d47e09de1b4d8f687a8dff2abf6aff1af0f21f
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777719"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="5b5a3-104">tipo complexo approvalSettings</span><span class="sxs-lookup"><span data-stu-id="5b5a3-104">approvalSettings complex type</span></span>

<span data-ttu-id="5b5a3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b5a3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b5a3-106">Usada para a `requestApprovalSettings` propriedade de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5b5a3-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="5b5a3-107">Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="5b5a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b5a3-108">Properties</span></span>

| <span data-ttu-id="5b5a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b5a3-109">Property</span></span>                     | <span data-ttu-id="5b5a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b5a3-110">Type</span></span>                      | <span data-ttu-id="5b5a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b5a3-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="5b5a3-112">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="5b5a3-112">isApprovalRequired</span></span> | <span data-ttu-id="5b5a3-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b5a3-113">Boolean</span></span> | <span data-ttu-id="5b5a3-114">Se for false, a aprovação não será necessária para solicitações nesta política.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="5b5a3-115">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="5b5a3-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="5b5a3-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b5a3-116">Boolean</span></span>| <span data-ttu-id="5b5a3-117">Se for false, a aprovação não será necessária para um usuário que já tenha uma atribuição para estender sua atribuição.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="5b5a3-118">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="5b5a3-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="5b5a3-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b5a3-119">Boolean</span></span> | <span data-ttu-id="5b5a3-120">Indica se o solicitante é necessário para fornecer uma justificativa em sua solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="5b5a3-121">approvalmode</span><span class="sxs-lookup"><span data-stu-id="5b5a3-121">approvalMode</span></span>| <span data-ttu-id="5b5a3-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b5a3-122">String</span></span> | <span data-ttu-id="5b5a3-123">Um de `NoApproval` , `SingleStage` ou `Serial` .</span><span class="sxs-lookup"><span data-stu-id="5b5a3-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="5b5a3-124">O `NoApproval` é usado quando `isApprovalRequired` é falso.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="5b5a3-125">approvalStages</span><span class="sxs-lookup"><span data-stu-id="5b5a3-125">approvalStages</span></span> | <span data-ttu-id="5b5a3-126">coleção [approvalStage](approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="5b5a3-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="5b5a3-127">Se for necessário aprovar, um ou dois elementos dessa coleção define cada um dos estágios de aprovação.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="5b5a3-128">Uma matriz vazia se nenhuma aprovação for necessária.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5b5a3-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b5a3-129">JSON representation</span></span>

<span data-ttu-id="5b5a3-130">Veja a seguir uma representação JSON da propriedade solicitar configurações de aprovação.</span><span class="sxs-lookup"><span data-stu-id="5b5a3-130">The following is a JSON representation of the request approval settings property.</span></span>

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


