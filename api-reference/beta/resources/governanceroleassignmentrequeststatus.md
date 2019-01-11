---
title: tipo de recurso de governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: c5daac53661cc607d51e5bfd1ec9031cfa599fca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808068"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="f75e2-103">tipo de recurso de governanceRoleAssignmentRequestStatus</span><span class="sxs-lookup"><span data-stu-id="f75e2-103">governanceRoleAssignmentRequestStatus resource type</span></span>

> <span data-ttu-id="f75e2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f75e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f75e2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f75e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f75e2-106">Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f75e2-106">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="f75e2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f75e2-107">Properties</span></span>
<span data-ttu-id="f75e2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f75e2-108">Property</span></span>       | <span data-ttu-id="f75e2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f75e2-109">Type</span></span> |<span data-ttu-id="f75e2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f75e2-110">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="f75e2-111">status</span><span class="sxs-lookup"><span data-stu-id="f75e2-111">status</span></span> |<span data-ttu-id="f75e2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f75e2-112">String</span></span>| <span data-ttu-id="f75e2-113">O status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f75e2-113">The status of the role assignment request.</span></span> <span data-ttu-id="f75e2-114">O valor pode ser `InProgress` ou `Closed`.</span><span class="sxs-lookup"><span data-stu-id="f75e2-114">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="f75e2-115">subStatus</span><span class="sxs-lookup"><span data-stu-id="f75e2-115">subStatus</span></span> |<span data-ttu-id="f75e2-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f75e2-116">String</span></span>| <span data-ttu-id="f75e2-117">O status de sub da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f75e2-117">The sub status of the role assignment request.</span></span> <span data-ttu-id="f75e2-118">Os valores podem ser `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, e `ProvisioningStarted`.</span><span class="sxs-lookup"><span data-stu-id="f75e2-118">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="f75e2-119">statusDetails</span><span class="sxs-lookup"><span data-stu-id="f75e2-119">statusDetails</span></span>       |<span data-ttu-id="f75e2-120">coleção [keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f75e2-120">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="f75e2-121">Os detalhes do status da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f75e2-121">The details of the status of the role assignment request.</span></span> <span data-ttu-id="f75e2-122">Ele representa os resultados de avaliação de regras diferentes.</span><span class="sxs-lookup"><span data-stu-id="f75e2-122">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f75e2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f75e2-123">JSON representation</span></span>

<span data-ttu-id="f75e2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f75e2-124">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
