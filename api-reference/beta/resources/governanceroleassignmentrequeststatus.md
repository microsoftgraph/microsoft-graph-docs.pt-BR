---
title: tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: a1031429d6288ec19a9f3791e24a35dc0d431588
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809501"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="ccce5-103">tipo de recurso governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="ccce5-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="ccce5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccce5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccce5-105">Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="ccce5-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="ccce5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccce5-106">Properties</span></span>
<span data-ttu-id="ccce5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccce5-107">Property</span></span>       | <span data-ttu-id="ccce5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccce5-108">Type</span></span> |<span data-ttu-id="ccce5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccce5-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="ccce5-110">status</span><span class="sxs-lookup"><span data-stu-id="ccce5-110">status</span></span> |<span data-ttu-id="ccce5-111">String</span><span class="sxs-lookup"><span data-stu-id="ccce5-111">String</span></span>| <span data-ttu-id="ccce5-112">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ccce5-112">The status of the role assignment request.</span></span> <span data-ttu-id="ccce5-113">O valor pode ser `InProgress` ou `Closed` .</span><span class="sxs-lookup"><span data-stu-id="ccce5-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="ccce5-114">substatus</span><span class="sxs-lookup"><span data-stu-id="ccce5-114">subStatus</span></span> |<span data-ttu-id="ccce5-115">String</span><span class="sxs-lookup"><span data-stu-id="ccce5-115">String</span></span>| <span data-ttu-id="ccce5-116">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ccce5-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="ccce5-117">Os valores podem ser,,,,,,,, `Accepted` `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` , `PendingApprovalProvisioning` ,, `PendingApproval` `FailedAsResourceIsLocked` , `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` ,,, e.</span><span class="sxs-lookup"><span data-stu-id="ccce5-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="ccce5-118">statusDetails</span><span class="sxs-lookup"><span data-stu-id="ccce5-118">statusDetails</span></span>       |<span data-ttu-id="ccce5-119">Coleção [KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ccce5-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="ccce5-120">Os detalhes do status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ccce5-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="ccce5-121">Ele representa os resultados de avaliação de regras diferentes.</span><span class="sxs-lookup"><span data-stu-id="ccce5-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccce5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccce5-122">JSON representation</span></span>

<span data-ttu-id="ccce5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccce5-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
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
  "suppressions": []
}
-->
