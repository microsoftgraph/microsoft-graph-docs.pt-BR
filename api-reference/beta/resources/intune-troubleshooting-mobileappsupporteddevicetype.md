---
title: tipo de recurso de mobileAppSupportedDeviceType
description: Propriedades do dispositivo
ms.openlocfilehash: 7bea84a009d8940608c82bbb551c2d3c8be750ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035508"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="f9cb8-103">tipo de recurso de mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="f9cb8-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="f9cb8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9cb8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9cb8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9cb8-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f9cb8-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="f9cb8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9cb8-108">Properties</span></span>
|<span data-ttu-id="f9cb8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9cb8-109">Property</span></span>|<span data-ttu-id="f9cb8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9cb8-110">Type</span></span>|<span data-ttu-id="f9cb8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9cb8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9cb8-112">type</span><span class="sxs-lookup"><span data-stu-id="f9cb8-112">type</span></span>|[<span data-ttu-id="f9cb8-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="f9cb8-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f9cb8-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-114">Device type.</span></span> <span data-ttu-id="f9cb8-115">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f9cb8-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f9cb8-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="f9cb8-117">String</span><span class="sxs-lookup"><span data-stu-id="f9cb8-117">String</span></span>|<span data-ttu-id="f9cb8-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f9cb8-118">Minimum OS version</span></span>|
|<span data-ttu-id="f9cb8-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f9cb8-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="f9cb8-120">String</span><span class="sxs-lookup"><span data-stu-id="f9cb8-120">String</span></span>|<span data-ttu-id="f9cb8-121">Versão de sistema operacional máxima</span><span class="sxs-lookup"><span data-stu-id="f9cb8-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9cb8-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f9cb8-122">Relationships</span></span>
<span data-ttu-id="f9cb8-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9cb8-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9cb8-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9cb8-124">JSON Representation</span></span>
<span data-ttu-id="f9cb8-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9cb8-125">Here is a JSON representation of the resource.</span></span>
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





