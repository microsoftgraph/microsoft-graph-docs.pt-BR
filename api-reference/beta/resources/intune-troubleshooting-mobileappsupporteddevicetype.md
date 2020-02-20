---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b71c9ec708efb36f677e563992eca4130f347c80
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159066"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="169b4-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="169b4-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="169b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="169b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="169b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="169b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="169b4-106">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="169b4-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="169b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="169b4-107">Properties</span></span>
|<span data-ttu-id="169b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="169b4-108">Property</span></span>|<span data-ttu-id="169b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="169b4-109">Type</span></span>|<span data-ttu-id="169b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="169b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="169b4-111">type</span><span class="sxs-lookup"><span data-stu-id="169b4-111">type</span></span>|[<span data-ttu-id="169b4-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="169b4-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="169b4-113">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="169b4-113">Device type.</span></span> <span data-ttu-id="169b4-114">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="169b4-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="169b4-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="169b4-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="169b4-116">String</span><span class="sxs-lookup"><span data-stu-id="169b4-116">String</span></span>|<span data-ttu-id="169b4-117">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="169b4-117">Minimum OS version</span></span>|
|<span data-ttu-id="169b4-118">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="169b4-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="169b4-119">String</span><span class="sxs-lookup"><span data-stu-id="169b4-119">String</span></span>|<span data-ttu-id="169b4-120">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="169b4-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="169b4-121">Relações</span><span class="sxs-lookup"><span data-stu-id="169b4-121">Relationships</span></span>
<span data-ttu-id="169b4-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="169b4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="169b4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="169b4-123">JSON Representation</span></span>
<span data-ttu-id="169b4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="169b4-124">Here is a JSON representation of the resource.</span></span>
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



