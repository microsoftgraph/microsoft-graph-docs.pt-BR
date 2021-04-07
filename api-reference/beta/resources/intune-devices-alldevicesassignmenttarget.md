---
title: Tipo de recurso allDevicesAssignmentTarget
description: Representa uma atribuição para todos os dispositivos gerenciados no locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ca3d3b4dbbe534189c66eba09ecbc6e99258936
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612117"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="16184-103">Tipo de recurso allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="16184-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="16184-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16184-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16184-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16184-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16184-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16184-107">Representa uma atribuição para todos os dispositivos gerenciados no locatário.</span><span class="sxs-lookup"><span data-stu-id="16184-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="16184-108">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="16184-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16184-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16184-109">Properties</span></span>
|<span data-ttu-id="16184-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16184-110">Property</span></span>|<span data-ttu-id="16184-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="16184-111">Type</span></span>|<span data-ttu-id="16184-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16184-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16184-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="16184-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="16184-114">String</span><span class="sxs-lookup"><span data-stu-id="16184-114">String</span></span>|<span data-ttu-id="16184-115">A ID do filtro para a atribuição de destino.</span><span class="sxs-lookup"><span data-stu-id="16184-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="16184-116">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="16184-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="16184-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="16184-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="16184-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="16184-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="16184-119">O tipo de filtro da atribuição de destino ou seja, Excluir ou Incluir.</span><span class="sxs-lookup"><span data-stu-id="16184-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="16184-120">Herdado [de deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="16184-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="16184-121">Os valores possíveis são: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="16184-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16184-122">Relações</span><span class="sxs-lookup"><span data-stu-id="16184-122">Relationships</span></span>
<span data-ttu-id="16184-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16184-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16184-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16184-124">JSON Representation</span></span>
<span data-ttu-id="16184-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16184-125">Here is a JSON representation of the resource.</span></span>
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




