---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cee2a17eb6cacab64488693f3a6a6580f3fb3264
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317777"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="d6d13-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="d6d13-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="d6d13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6d13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6d13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6d13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6d13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d13-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d6d13-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="d6d13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6d13-108">Properties</span></span>
|<span data-ttu-id="d6d13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6d13-109">Property</span></span>|<span data-ttu-id="d6d13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6d13-110">Type</span></span>|<span data-ttu-id="d6d13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6d13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d13-112">type</span><span class="sxs-lookup"><span data-stu-id="d6d13-112">type</span></span>|[<span data-ttu-id="d6d13-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="d6d13-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d6d13-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6d13-114">Device type.</span></span> <span data-ttu-id="d6d13-115">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="d6d13-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d6d13-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d6d13-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="d6d13-117">String</span><span class="sxs-lookup"><span data-stu-id="d6d13-117">String</span></span>|<span data-ttu-id="d6d13-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d6d13-118">Minimum OS version</span></span>|
|<span data-ttu-id="d6d13-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d6d13-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="d6d13-120">String</span><span class="sxs-lookup"><span data-stu-id="d6d13-120">String</span></span>|<span data-ttu-id="d6d13-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d6d13-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6d13-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d6d13-122">Relationships</span></span>
<span data-ttu-id="d6d13-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6d13-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6d13-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6d13-124">JSON Representation</span></span>
<span data-ttu-id="d6d13-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6d13-125">Here is a JSON representation of the resource.</span></span>
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



