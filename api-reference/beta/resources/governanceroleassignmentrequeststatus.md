---
title: tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca61e5e3ef5456889eafcef3914f16fc072dfb6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971854"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="3e80d-103">tipo de recurso governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="3e80d-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e80d-104">Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="3e80d-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="3e80d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e80d-105">Properties</span></span>
<span data-ttu-id="3e80d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e80d-106">Property</span></span>       | <span data-ttu-id="3e80d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e80d-107">Type</span></span> |<span data-ttu-id="3e80d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e80d-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="3e80d-109">status</span><span class="sxs-lookup"><span data-stu-id="3e80d-109">status</span></span> |<span data-ttu-id="3e80d-110">String</span><span class="sxs-lookup"><span data-stu-id="3e80d-110">String</span></span>| <span data-ttu-id="3e80d-111">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3e80d-111">The status of the role assignment request.</span></span> <span data-ttu-id="3e80d-112">O valor pode ser `InProgress` ou `Closed`.</span><span class="sxs-lookup"><span data-stu-id="3e80d-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="3e80d-113">substatus</span><span class="sxs-lookup"><span data-stu-id="3e80d-113">subStatus</span></span> |<span data-ttu-id="3e80d-114">String</span><span class="sxs-lookup"><span data-stu-id="3e80d-114">String</span></span>| <span data-ttu-id="3e80d-115">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3e80d-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="3e80d-116">Os valores podem ser `Accepted`, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `AdminApproved` `AdminDenied` `PendingAdminDecision` `PendingApproval` `Failed` `PendingApprovalProvisioning` `FailedAsResourceIsLocked` `TimedOut`,,,,,,,,,,,,,, e `ProvisioningStarted` `PendingRevocation` `Revoked` `Canceled`</span><span class="sxs-lookup"><span data-stu-id="3e80d-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="3e80d-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="3e80d-117">statusDetails</span></span>       |<span data-ttu-id="3e80d-118">Coleção [KeyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3e80d-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="3e80d-119">Os detalhes do status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3e80d-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="3e80d-120">Ele representa os resultados de avaliação de regras diferentes.</span><span class="sxs-lookup"><span data-stu-id="3e80d-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e80d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e80d-121">JSON representation</span></span>

<span data-ttu-id="3e80d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e80d-122">Here is a JSON representation of the resource.</span></span>

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
