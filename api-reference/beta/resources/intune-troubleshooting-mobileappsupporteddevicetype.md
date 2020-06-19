---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 787a51b2fb336c19598f89bcc875558f8eb0d291
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793737"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="aa8b3-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="aa8b3-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="aa8b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa8b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa8b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa8b3-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aa8b3-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="aa8b3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa8b3-108">Properties</span></span>
|<span data-ttu-id="aa8b3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa8b3-109">Property</span></span>|<span data-ttu-id="aa8b3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa8b3-110">Type</span></span>|<span data-ttu-id="aa8b3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8b3-112">type</span><span class="sxs-lookup"><span data-stu-id="aa8b3-112">type</span></span>|[<span data-ttu-id="aa8b3-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="aa8b3-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="aa8b3-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-114">Device type.</span></span> <span data-ttu-id="aa8b3-115">Os valores possíveis são:,,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` , `holoLens` , `surfaceHub` , `androidForWork` , `androidEnterprise` , `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="aa8b3-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="aa8b3-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="aa8b3-117">String</span><span class="sxs-lookup"><span data-stu-id="aa8b3-117">String</span></span>|<span data-ttu-id="aa8b3-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="aa8b3-118">Minimum OS version</span></span>|
|<span data-ttu-id="aa8b3-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="aa8b3-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="aa8b3-120">String</span><span class="sxs-lookup"><span data-stu-id="aa8b3-120">String</span></span>|<span data-ttu-id="aa8b3-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="aa8b3-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa8b3-122">Relações</span><span class="sxs-lookup"><span data-stu-id="aa8b3-122">Relationships</span></span>
<span data-ttu-id="aa8b3-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="aa8b3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa8b3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa8b3-124">JSON Representation</span></span>
<span data-ttu-id="aa8b3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa8b3-125">Here is a JSON representation of the resource.</span></span>
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



