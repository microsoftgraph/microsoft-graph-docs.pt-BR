---
title: Tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 559dc38a5fc8d2e9b7142efb43d83a97f29db10c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141376"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="a349e-103">Tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="a349e-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="a349e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a349e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a349e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a349e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a349e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a349e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a349e-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a349e-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="a349e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a349e-108">Properties</span></span>
|<span data-ttu-id="a349e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a349e-109">Property</span></span>|<span data-ttu-id="a349e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a349e-110">Type</span></span>|<span data-ttu-id="a349e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a349e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a349e-112">type</span><span class="sxs-lookup"><span data-stu-id="a349e-112">type</span></span>|[<span data-ttu-id="a349e-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="a349e-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a349e-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a349e-114">Device type.</span></span> <span data-ttu-id="a349e-115">Os valores possíveis são: `desktop` , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="a349e-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="a349e-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a349e-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="a349e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a349e-117">String</span></span>|<span data-ttu-id="a349e-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a349e-118">Minimum OS version</span></span>|
|<span data-ttu-id="a349e-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a349e-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="a349e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a349e-120">String</span></span>|<span data-ttu-id="a349e-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a349e-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="a349e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="a349e-122">Relationships</span></span>
<span data-ttu-id="a349e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a349e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a349e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a349e-124">JSON Representation</span></span>
<span data-ttu-id="a349e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a349e-125">Here is a JSON representation of the resource.</span></span>
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




