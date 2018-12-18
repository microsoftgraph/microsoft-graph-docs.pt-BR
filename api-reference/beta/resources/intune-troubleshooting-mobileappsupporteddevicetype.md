---
title: tipo de recurso de mobileAppSupportedDeviceType
description: Propriedades do dispositivo
author: tfitzmac
ms.openlocfilehash: 5ec7d2b1e8340b73ea184dda15d842973f0fab2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314417"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="7759b-103">tipo de recurso de mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="7759b-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="7759b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7759b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7759b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7759b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7759b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7759b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7759b-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7759b-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="7759b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7759b-108">Properties</span></span>
|<span data-ttu-id="7759b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7759b-109">Property</span></span>|<span data-ttu-id="7759b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7759b-110">Type</span></span>|<span data-ttu-id="7759b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7759b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7759b-112">type</span><span class="sxs-lookup"><span data-stu-id="7759b-112">type</span></span>|[<span data-ttu-id="7759b-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="7759b-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="7759b-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7759b-114">Device type.</span></span> <span data-ttu-id="7759b-115">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7759b-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7759b-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7759b-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="7759b-117">String</span><span class="sxs-lookup"><span data-stu-id="7759b-117">String</span></span>|<span data-ttu-id="7759b-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7759b-118">Minimum OS version</span></span>|
|<span data-ttu-id="7759b-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7759b-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="7759b-120">String</span><span class="sxs-lookup"><span data-stu-id="7759b-120">String</span></span>|<span data-ttu-id="7759b-121">Versão de sistema operacional máxima</span><span class="sxs-lookup"><span data-stu-id="7759b-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="7759b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="7759b-122">Relationships</span></span>
<span data-ttu-id="7759b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7759b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7759b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7759b-124">JSON Representation</span></span>
<span data-ttu-id="7759b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7759b-125">Here is a JSON representation of the resource.</span></span>
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





