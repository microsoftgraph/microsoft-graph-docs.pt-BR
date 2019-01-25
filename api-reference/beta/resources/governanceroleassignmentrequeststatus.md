---
title: tipo de recurso de governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510173"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="db8e2-103">tipo de recurso de governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="db8e2-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db8e2-104">Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="db8e2-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="db8e2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db8e2-105">Properties</span></span>
<span data-ttu-id="db8e2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db8e2-106">Property</span></span>       | <span data-ttu-id="db8e2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="db8e2-107">Type</span></span> |<span data-ttu-id="db8e2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="db8e2-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="db8e2-109">status</span><span class="sxs-lookup"><span data-stu-id="db8e2-109">status</span></span> |<span data-ttu-id="db8e2-110">String</span><span class="sxs-lookup"><span data-stu-id="db8e2-110">String</span></span>| <span data-ttu-id="db8e2-111">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="db8e2-111">The status of the role assignment request.</span></span> <span data-ttu-id="db8e2-112">O valor pode ser `InProgress` ou `Closed`.</span><span class="sxs-lookup"><span data-stu-id="db8e2-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="db8e2-113">subStatus</span><span class="sxs-lookup"><span data-stu-id="db8e2-113">subStatus</span></span> |<span data-ttu-id="db8e2-114">String</span><span class="sxs-lookup"><span data-stu-id="db8e2-114">String</span></span>| <span data-ttu-id="db8e2-115">O status de sub da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="db8e2-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="db8e2-116">Os valores podem ser `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, e `ProvisioningStarted`.</span><span class="sxs-lookup"><span data-stu-id="db8e2-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="db8e2-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="db8e2-117">statusDetails</span></span>       |<span data-ttu-id="db8e2-118">coleção [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="db8e2-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="db8e2-119">Os detalhes do status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="db8e2-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="db8e2-120">Ele representa os resultados de avaliação de regras diferentes.</span><span class="sxs-lookup"><span data-stu-id="db8e2-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db8e2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db8e2-121">JSON representation</span></span>

<span data-ttu-id="db8e2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db8e2-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
