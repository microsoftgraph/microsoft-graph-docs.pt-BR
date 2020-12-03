---
title: tipo de recurso cloudPcProvisioningPolicyAssignment
description: Atribuições de política de provisionamento do CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563692"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="80c27-103">tipo de recurso cloudPcProvisioningPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="80c27-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="80c27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80c27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80c27-105">Representa uma coleção definida de atribuições de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="80c27-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="80c27-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80c27-106">Properties</span></span>

|<span data-ttu-id="80c27-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80c27-107">Property</span></span>|<span data-ttu-id="80c27-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="80c27-108">Type</span></span>|<span data-ttu-id="80c27-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="80c27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c27-110">id</span><span class="sxs-lookup"><span data-stu-id="80c27-110">id</span></span>|<span data-ttu-id="80c27-111">String</span><span class="sxs-lookup"><span data-stu-id="80c27-111">String</span></span>|<span data-ttu-id="80c27-112">Identificador exclusivo da atribuição de política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="80c27-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="80c27-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80c27-113">Read-only.</span></span> <span data-ttu-id="80c27-114">Se `target` for um grupo de usuários, a ID será mostrada como {PolicyId} _ {GroupId}.</span><span class="sxs-lookup"><span data-stu-id="80c27-114">If `target` is a user group, then the ID is shown as {policyId}_{groupId}.</span></span>|
|<span data-ttu-id="80c27-115">destino</span><span class="sxs-lookup"><span data-stu-id="80c27-115">target</span></span>|[<span data-ttu-id="80c27-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="80c27-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="80c27-117">O destino da atribuição para a política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="80c27-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="80c27-118">Atualmente, o único destino com suporte para essa política é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="80c27-118">Currently, the only target supported for this policy is a user group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80c27-119">Relações</span><span class="sxs-lookup"><span data-stu-id="80c27-119">Relationships</span></span>

<span data-ttu-id="80c27-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80c27-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80c27-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80c27-121">JSON representation</span></span>

<span data-ttu-id="80c27-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80c27-122">The following is a JSON representation of the resource.</span></span>
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
