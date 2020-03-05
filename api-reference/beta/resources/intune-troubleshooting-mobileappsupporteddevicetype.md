---
title: tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8e0b0f6232645dfff0e59e8d1ff808e47ff472
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523321"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="f0134-103">tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="f0134-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="f0134-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f0134-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0134-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0134-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0134-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0134-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0134-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f0134-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="f0134-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0134-108">Properties</span></span>
|<span data-ttu-id="f0134-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0134-109">Property</span></span>|<span data-ttu-id="f0134-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0134-110">Type</span></span>|<span data-ttu-id="f0134-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0134-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0134-112">type</span><span class="sxs-lookup"><span data-stu-id="f0134-112">type</span></span>|[<span data-ttu-id="f0134-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="f0134-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f0134-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0134-114">Device type.</span></span> <span data-ttu-id="f0134-115">Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="f0134-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f0134-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f0134-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="f0134-117">String</span><span class="sxs-lookup"><span data-stu-id="f0134-117">String</span></span>|<span data-ttu-id="f0134-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f0134-118">Minimum OS version</span></span>|
|<span data-ttu-id="f0134-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f0134-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="f0134-120">String</span><span class="sxs-lookup"><span data-stu-id="f0134-120">String</span></span>|<span data-ttu-id="f0134-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f0134-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0134-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f0134-122">Relationships</span></span>
<span data-ttu-id="f0134-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0134-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0134-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0134-124">JSON Representation</span></span>
<span data-ttu-id="f0134-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0134-125">Here is a JSON representation of the resource.</span></span>
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



