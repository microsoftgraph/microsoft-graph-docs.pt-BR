---
title: tipo de recurso cloudPcManagementGroupAssignmentTarget
description: 'Tipo complexo que representa o grupo de destino de atribuição. Tipo de base: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378264"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="542a9-104">tipo de recurso cloudPcManagementGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="542a9-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="542a9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="542a9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="542a9-106">Tipo complexo que representa o grupo de destino de atribuição.</span><span class="sxs-lookup"><span data-stu-id="542a9-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="542a9-107">Herda de [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="542a9-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="542a9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="542a9-108">Properties</span></span>

|<span data-ttu-id="542a9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="542a9-109">Property</span></span>|<span data-ttu-id="542a9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="542a9-110">Type</span></span>|<span data-ttu-id="542a9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="542a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542a9-112">groupId</span><span class="sxs-lookup"><span data-stu-id="542a9-112">groupId</span></span>|<span data-ttu-id="542a9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="542a9-113">String</span></span>|<span data-ttu-id="542a9-114">A ID do grupo de destino da atribuição</span><span class="sxs-lookup"><span data-stu-id="542a9-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="542a9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="542a9-115">Relationships</span></span>

<span data-ttu-id="542a9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="542a9-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="542a9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="542a9-117">JSON representation</span></span>

<span data-ttu-id="542a9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="542a9-118">The following is a JSON representation of the resource.</span></span>
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
