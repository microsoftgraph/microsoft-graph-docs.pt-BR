---
title: Tipo de recurso mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a3e2fc78712997eebd31a874363f000b4ad761e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863566"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="fe036-103">Tipo de recurso mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="fe036-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="fe036-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe036-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe036-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe036-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe036-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe036-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe036-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fe036-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="fe036-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe036-108">Properties</span></span>
|<span data-ttu-id="fe036-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe036-109">Property</span></span>|<span data-ttu-id="fe036-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe036-110">Type</span></span>|<span data-ttu-id="fe036-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe036-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe036-112">type</span><span class="sxs-lookup"><span data-stu-id="fe036-112">type</span></span>|[<span data-ttu-id="fe036-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="fe036-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="fe036-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe036-114">Device type.</span></span> <span data-ttu-id="fe036-115">Os valores possíveis são: `desktop` , , , , , , , , `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` , `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC`</span><span class="sxs-lookup"><span data-stu-id="fe036-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="fe036-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fe036-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="fe036-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fe036-117">String</span></span>|<span data-ttu-id="fe036-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="fe036-118">Minimum OS version</span></span>|
|<span data-ttu-id="fe036-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fe036-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="fe036-120">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fe036-120">String</span></span>|<span data-ttu-id="fe036-121">Versão máxima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="fe036-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe036-122">Relações</span><span class="sxs-lookup"><span data-stu-id="fe036-122">Relationships</span></span>
<span data-ttu-id="fe036-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe036-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe036-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe036-124">JSON Representation</span></span>
<span data-ttu-id="fe036-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe036-125">Here is a JSON representation of the resource.</span></span>
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




