---
title: tipo de recurso de mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1b757e9c621f77d1a26251345ee6751eca2ca7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980220"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="5af66-103">tipo de recurso de mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="5af66-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="5af66-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5af66-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5af66-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5af66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af66-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5af66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5af66-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5af66-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="5af66-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5af66-108">Properties</span></span>
|<span data-ttu-id="5af66-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5af66-109">Property</span></span>|<span data-ttu-id="5af66-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5af66-110">Type</span></span>|<span data-ttu-id="5af66-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5af66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af66-112">type</span><span class="sxs-lookup"><span data-stu-id="5af66-112">type</span></span>|[<span data-ttu-id="5af66-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="5af66-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5af66-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5af66-114">Device type.</span></span> <span data-ttu-id="5af66-115">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5af66-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5af66-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="5af66-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="5af66-117">String</span><span class="sxs-lookup"><span data-stu-id="5af66-117">String</span></span>|<span data-ttu-id="5af66-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5af66-118">Minimum OS version</span></span>|
|<span data-ttu-id="5af66-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="5af66-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="5af66-120">String</span><span class="sxs-lookup"><span data-stu-id="5af66-120">String</span></span>|<span data-ttu-id="5af66-121">Versão de sistema operacional máxima</span><span class="sxs-lookup"><span data-stu-id="5af66-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="5af66-122">Relações</span><span class="sxs-lookup"><span data-stu-id="5af66-122">Relationships</span></span>
<span data-ttu-id="5af66-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5af66-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5af66-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5af66-124">JSON Representation</span></span>
<span data-ttu-id="5af66-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5af66-125">Here is a JSON representation of the resource.</span></span>
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





