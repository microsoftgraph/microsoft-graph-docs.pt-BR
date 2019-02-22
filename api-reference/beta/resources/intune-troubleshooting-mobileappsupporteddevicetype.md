---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76b3ca431bc68f93144a33dd8c5e8e5f036764a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140576"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="77e3c-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="77e3c-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="77e3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77e3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77e3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77e3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77e3c-106">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="77e3c-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="77e3c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77e3c-107">Properties</span></span>
|<span data-ttu-id="77e3c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77e3c-108">Property</span></span>|<span data-ttu-id="77e3c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="77e3c-109">Type</span></span>|<span data-ttu-id="77e3c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="77e3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77e3c-111">type</span><span class="sxs-lookup"><span data-stu-id="77e3c-111">type</span></span>|[<span data-ttu-id="77e3c-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="77e3c-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="77e3c-113">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77e3c-113">Device type.</span></span> <span data-ttu-id="77e3c-114">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="77e3c-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="77e3c-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="77e3c-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="77e3c-116">String</span><span class="sxs-lookup"><span data-stu-id="77e3c-116">String</span></span>|<span data-ttu-id="77e3c-117">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="77e3c-117">Minimum OS version</span></span>|
|<span data-ttu-id="77e3c-118">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="77e3c-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="77e3c-119">String</span><span class="sxs-lookup"><span data-stu-id="77e3c-119">String</span></span>|<span data-ttu-id="77e3c-120">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="77e3c-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="77e3c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="77e3c-121">Relationships</span></span>
<span data-ttu-id="77e3c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77e3c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77e3c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77e3c-123">JSON Representation</span></span>
<span data-ttu-id="77e3c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77e3c-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```




