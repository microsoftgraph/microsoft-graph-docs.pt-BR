---
title: Tipo de recurso cloudPcProvisioningPolicyAssignment
description: Atribuições de política de provisionamento do CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a96c3717b97b3f721c77b1150841f1eb51ded89f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082234"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="a6491-103">Tipo de recurso cloudPcProvisioningPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a6491-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="a6491-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6491-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6491-105">Representa uma coleção definida de atribuições de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="a6491-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="a6491-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6491-106">Properties</span></span>

|<span data-ttu-id="a6491-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6491-107">Property</span></span>|<span data-ttu-id="a6491-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6491-108">Type</span></span>|<span data-ttu-id="a6491-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6491-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6491-110">id</span><span class="sxs-lookup"><span data-stu-id="a6491-110">id</span></span>|<span data-ttu-id="a6491-111">String</span><span class="sxs-lookup"><span data-stu-id="a6491-111">String</span></span>|<span data-ttu-id="a6491-112">Identificador exclusivo para a atribuição de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="a6491-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="a6491-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6491-113">Read-only.</span></span> <span data-ttu-id="a6491-114">Se `target` for um grupo de usuários, a ID será mostrada como {policyId} \_ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="a6491-114">If `target` is a user group, then the ID is shown as {policyId}\_{groupId}.</span></span>|
|<span data-ttu-id="a6491-115">destino</span><span class="sxs-lookup"><span data-stu-id="a6491-115">target</span></span>|[<span data-ttu-id="a6491-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a6491-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="a6491-117">O destino da atribuição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="a6491-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="a6491-118">Atualmente, o único destino com suporte para essa política é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="a6491-118">Currently, the only target supported for this policy is a user group.</span></span> <span data-ttu-id="a6491-119">Para obter detalhes, [consulte cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="a6491-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a6491-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a6491-120">Relationships</span></span>

<span data-ttu-id="a6491-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6491-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6491-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6491-122">JSON representation</span></span>

<span data-ttu-id="a6491-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6491-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
