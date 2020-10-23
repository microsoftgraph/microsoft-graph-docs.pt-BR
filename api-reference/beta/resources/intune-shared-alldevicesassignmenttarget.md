---
title: Tipo de recurso allDevicesAssignmentTarget
description: Representa uma atribuição para todos os dispositivos gerenciados no locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba478c5505796f9039b6ab121fbbd5f9bf30edd4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733158"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="c6ce0-103">Tipo de recurso allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c6ce0-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="c6ce0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6ce0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6ce0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6ce0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6ce0-107">Representa uma atribuição para todos os dispositivos gerenciados no locatário.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="c6ce0-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c6ce0-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6ce0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6ce0-109">Properties</span></span>
|<span data-ttu-id="c6ce0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6ce0-110">Property</span></span>|<span data-ttu-id="c6ce0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6ce0-111">Type</span></span>|<span data-ttu-id="c6ce0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6ce0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ce0-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="c6ce0-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="c6ce0-114">String</span><span class="sxs-lookup"><span data-stu-id="c6ce0-114">String</span></span>|<span data-ttu-id="c6ce0-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="c6ce0-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c6ce0-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="c6ce0-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="c6ce0-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="c6ce0-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="c6ce0-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="c6ce0-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="c6ce0-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="c6ce0-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="c6ce0-121">Os valores possíveis são: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ce0-122">Relações</span><span class="sxs-lookup"><span data-stu-id="c6ce0-122">Relationships</span></span>
<span data-ttu-id="c6ce0-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6ce0-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6ce0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6ce0-124">JSON Representation</span></span>
<span data-ttu-id="c6ce0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6ce0-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allDevicesAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```





