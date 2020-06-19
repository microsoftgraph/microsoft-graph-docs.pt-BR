---
title: tipo de recurso deviceManagementPartnerAssignment
description: Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23094519b0271e60bdafb33e8c95eb103510451e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788875"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="9303f-103">tipo de recurso deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="9303f-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="9303f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9303f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9303f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9303f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9303f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9303f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9303f-107">Direcionamento de grupo de usuários para o parceiro de gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9303f-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="9303f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9303f-108">Properties</span></span>
|<span data-ttu-id="9303f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9303f-109">Property</span></span>|<span data-ttu-id="9303f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9303f-110">Type</span></span>|<span data-ttu-id="9303f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9303f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9303f-112">destino</span><span class="sxs-lookup"><span data-stu-id="9303f-112">target</span></span>|[<span data-ttu-id="9303f-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9303f-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9303f-114">Grupos de usuários direcionados a dispositivos a serem registrados por meio do parceiro.</span><span class="sxs-lookup"><span data-stu-id="9303f-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9303f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="9303f-115">Relationships</span></span>
<span data-ttu-id="9303f-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9303f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9303f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9303f-117">JSON Representation</span></span>
<span data-ttu-id="9303f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9303f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



