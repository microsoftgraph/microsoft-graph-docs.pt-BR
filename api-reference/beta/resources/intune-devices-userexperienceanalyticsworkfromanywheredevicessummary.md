---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary
description: O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6448bbc89ebe8357fa14a375f82fb73938f6634
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146733"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a><span data-ttu-id="d26b6-103">tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-103">userExperienceAnalyticsWorkFromAnywhereDevicesSummary resource type</span></span>

<span data-ttu-id="d26b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d26b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d26b6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d26b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d26b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d26b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d26b6-107">O resumo de dispositivos de métricas work from anywhere da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d26b6-107">The user experience analytics Work From Anywhere metrics devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="d26b6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d26b6-108">Properties</span></span>
|<span data-ttu-id="d26b6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d26b6-109">Property</span></span>|<span data-ttu-id="d26b6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d26b6-110">Type</span></span>|<span data-ttu-id="d26b6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d26b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d26b6-112">autopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-112">autopilotDevicesSummary</span></span>|[<span data-ttu-id="d26b6-113">userExperienceAnalyticsAutopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-113">userExperienceAnalyticsAutopilotDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|<span data-ttu-id="d26b6-114">O valor do trabalho de qualquer lugar resumo de dispositivos de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="d26b6-114">The value of work from anywhere autopilot devices summary.</span></span>|
|<span data-ttu-id="d26b6-115">cloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-115">cloudManagementDevicesSummary</span></span>|[<span data-ttu-id="d26b6-116">userExperienceAnalyticsCloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-116">userExperienceAnalyticsCloudManagementDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|<span data-ttu-id="d26b6-117">A experiência do usuário funciona de qualquer lugar Resumo de dispositivos de gerenciamento de nuvem.</span><span class="sxs-lookup"><span data-stu-id="d26b6-117">The user experience work from anywhere Cloud management devices summary.</span></span>|
|<span data-ttu-id="d26b6-118">windows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-118">windows10DevicesSummary</span></span>|[<span data-ttu-id="d26b6-119">userExperienceAnalyticsWindows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="d26b6-119">userExperienceAnalyticsWindows10DevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|<span data-ttu-id="d26b6-120">A análise da experiência do usuário funciona em qualquer lugar do resumo de dispositivos Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d26b6-120">The user experience analytics work from anywhere Windows 10 devices summary.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d26b6-121">Relações</span><span class="sxs-lookup"><span data-stu-id="d26b6-121">Relationships</span></span>
<span data-ttu-id="d26b6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d26b6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d26b6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d26b6-123">JSON Representation</span></span>
<span data-ttu-id="d26b6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d26b6-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
  "autopilotDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
    "devicesNotAutopilotRegistered": 1024,
    "devicesWithoutAutopilotProfileAssigned": 1024
  },
  "cloudManagementDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
    "coManagedDeviceCount": 1024,
    "intuneDeviceCount": 1024,
    "tenantAttachDeviceCount": 1024
  },
  "windows10DevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
    "unsupportedOSversionDeviceCount": 1024
  }
}
```




