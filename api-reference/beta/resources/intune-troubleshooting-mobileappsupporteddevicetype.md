---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: efd91d4ab3e4f267faf371cdb9ef3e828c59ffe1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764590"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="302c6-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="302c6-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="302c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="302c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="302c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="302c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="302c6-106">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="302c6-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="302c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="302c6-107">Properties</span></span>
|<span data-ttu-id="302c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="302c6-108">Property</span></span>|<span data-ttu-id="302c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="302c6-109">Type</span></span>|<span data-ttu-id="302c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="302c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="302c6-111">type</span><span class="sxs-lookup"><span data-stu-id="302c6-111">type</span></span>|[<span data-ttu-id="302c6-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="302c6-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="302c6-113">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="302c6-113">Device type.</span></span> <span data-ttu-id="302c6-114">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="302c6-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="302c6-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="302c6-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="302c6-116">String</span><span class="sxs-lookup"><span data-stu-id="302c6-116">String</span></span>|<span data-ttu-id="302c6-117">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="302c6-117">Minimum OS version</span></span>|
|<span data-ttu-id="302c6-118">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="302c6-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="302c6-119">String</span><span class="sxs-lookup"><span data-stu-id="302c6-119">String</span></span>|<span data-ttu-id="302c6-120">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="302c6-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="302c6-121">Relações</span><span class="sxs-lookup"><span data-stu-id="302c6-121">Relationships</span></span>
<span data-ttu-id="302c6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="302c6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="302c6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="302c6-123">JSON Representation</span></span>
<span data-ttu-id="302c6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="302c6-124">Here is a JSON representation of the resource.</span></span>
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



