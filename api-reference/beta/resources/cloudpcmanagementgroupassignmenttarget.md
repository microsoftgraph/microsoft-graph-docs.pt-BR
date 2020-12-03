---
title: tipo de recurso cloudPcManagementGroupAssignmentTarget
description: 'Tipo complexo que representa o grupo de destino de atribuição. Tipo de base: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563835"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="0e059-104">tipo de recurso cloudPcManagementGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0e059-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="0e059-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e059-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e059-106">Tipo complexo que representa o grupo de destino de atribuição.</span><span class="sxs-lookup"><span data-stu-id="0e059-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="0e059-107">Herda de [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="0e059-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="0e059-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e059-108">Properties</span></span>

|<span data-ttu-id="0e059-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e059-109">Property</span></span>|<span data-ttu-id="0e059-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e059-110">Type</span></span>|<span data-ttu-id="0e059-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e059-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e059-112">groupId</span><span class="sxs-lookup"><span data-stu-id="0e059-112">groupId</span></span>|<span data-ttu-id="0e059-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e059-113">String</span></span>|<span data-ttu-id="0e059-114">A ID do grupo de destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="0e059-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e059-115">Relações</span><span class="sxs-lookup"><span data-stu-id="0e059-115">Relationships</span></span>

<span data-ttu-id="0e059-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e059-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e059-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e059-117">JSON representation</span></span>

<span data-ttu-id="0e059-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e059-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
