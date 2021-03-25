---
title: tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary
description: O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159336"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a><span data-ttu-id="a5050-103">tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="a5050-103">userExperienceAnalyticsAutopilotDevicesSummary resource type</span></span>

<span data-ttu-id="a5050-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5050-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5050-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5050-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5050-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5050-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5050-107">O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.</span><span class="sxs-lookup"><span data-stu-id="a5050-107">The user experience analytics summary of Devices not windows autopilot ready.</span></span>

## <a name="properties"></a><span data-ttu-id="a5050-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5050-108">Properties</span></span>
|<span data-ttu-id="a5050-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5050-109">Property</span></span>|<span data-ttu-id="a5050-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5050-110">Type</span></span>|<span data-ttu-id="a5050-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5050-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5050-112">devicesNotAutopilotRegistered</span><span class="sxs-lookup"><span data-stu-id="a5050-112">devicesNotAutopilotRegistered</span></span>|<span data-ttu-id="a5050-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a5050-113">Int32</span></span>|<span data-ttu-id="a5050-114">A contagem de dispositivos do intune que não estão no piloto automático registrado.</span><span class="sxs-lookup"><span data-stu-id="a5050-114">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="a5050-115">devicesWithoutAutopilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="a5050-115">devicesWithoutAutopilotProfileAssigned</span></span>|<span data-ttu-id="a5050-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a5050-116">Int32</span></span>|<span data-ttu-id="a5050-117">A contagem de dispositivos do intune não atribuídos ao perfil de piloto automático.</span><span class="sxs-lookup"><span data-stu-id="a5050-117">The count of intune devices not autopilot profile assigned.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5050-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a5050-118">Relationships</span></span>
<span data-ttu-id="a5050-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5050-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5050-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5050-120">JSON Representation</span></span>
<span data-ttu-id="a5050-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5050-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




