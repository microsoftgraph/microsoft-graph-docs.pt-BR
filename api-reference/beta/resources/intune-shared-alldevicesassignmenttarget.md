---
title: Tipo de recurso allDevicesAssignmentTarget
description: Representa uma atribuição para todos os dispositivos gerenciados no locatário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69f5e1f77a1fed08d8139e63ffada76e3a948917
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793602"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="d9df3-103">Tipo de recurso allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9df3-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="d9df3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9df3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9df3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9df3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9df3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9df3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9df3-107">Representa uma atribuição para todos os dispositivos gerenciados no locatário.</span><span class="sxs-lookup"><span data-stu-id="d9df3-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="d9df3-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d9df3-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9df3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9df3-109">Properties</span></span>
|<span data-ttu-id="d9df3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9df3-110">Property</span></span>|<span data-ttu-id="d9df3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9df3-111">Type</span></span>|<span data-ttu-id="d9df3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9df3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9df3-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="d9df3-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="d9df3-114">String</span><span class="sxs-lookup"><span data-stu-id="d9df3-114">String</span></span>|<span data-ttu-id="d9df3-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="d9df3-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="d9df3-116">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d9df3-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="d9df3-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="d9df3-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="d9df3-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="d9df3-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="d9df3-119">O tipo de filtro da atribuição de destino, ou seja, excluir ou incluir.</span><span class="sxs-lookup"><span data-stu-id="d9df3-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="d9df3-120">Herdado de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="d9df3-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="d9df3-121">Os valores possíveis são: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="d9df3-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9df3-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d9df3-122">Relationships</span></span>
<span data-ttu-id="d9df3-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d9df3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9df3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9df3-124">JSON Representation</span></span>
<span data-ttu-id="d9df3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9df3-125">Here is a JSON representation of the resource.</span></span>
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



