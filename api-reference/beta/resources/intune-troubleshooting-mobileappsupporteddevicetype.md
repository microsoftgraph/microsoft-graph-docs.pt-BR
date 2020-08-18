---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef5d013492125b16b14f2fe2c3613549df3b537e
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791697"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="cc74b-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="cc74b-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="cc74b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc74b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc74b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc74b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc74b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc74b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc74b-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cc74b-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="cc74b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc74b-108">Properties</span></span>
|<span data-ttu-id="cc74b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc74b-109">Property</span></span>|<span data-ttu-id="cc74b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc74b-110">Type</span></span>|<span data-ttu-id="cc74b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc74b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc74b-112">type</span><span class="sxs-lookup"><span data-stu-id="cc74b-112">type</span></span>|[<span data-ttu-id="cc74b-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="cc74b-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="cc74b-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc74b-114">Device type.</span></span> <span data-ttu-id="cc74b-115">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="cc74b-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="cc74b-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cc74b-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="cc74b-117">String</span><span class="sxs-lookup"><span data-stu-id="cc74b-117">String</span></span>|<span data-ttu-id="cc74b-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="cc74b-118">Minimum OS version</span></span>|
|<span data-ttu-id="cc74b-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cc74b-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="cc74b-120">String</span><span class="sxs-lookup"><span data-stu-id="cc74b-120">String</span></span>|<span data-ttu-id="cc74b-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="cc74b-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc74b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="cc74b-122">Relationships</span></span>
<span data-ttu-id="cc74b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc74b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc74b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc74b-124">JSON Representation</span></span>
<span data-ttu-id="cc74b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc74b-125">Here is a JSON representation of the resource.</span></span>
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



