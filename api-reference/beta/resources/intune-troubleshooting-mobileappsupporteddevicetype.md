---
title: tipo de recurso de mobileAppSupportedDeviceType
description: Propriedades do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c01691b3f6fcb2ed5838c1c9103c99ad6fbe792f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399749"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="e80e7-103">tipo de recurso de mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="e80e7-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="e80e7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e80e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e80e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e80e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e80e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e80e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e80e7-107">Propriedades do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e80e7-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="e80e7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e80e7-108">Properties</span></span>
|<span data-ttu-id="e80e7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e80e7-109">Property</span></span>|<span data-ttu-id="e80e7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80e7-110">Type</span></span>|<span data-ttu-id="e80e7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e80e7-112">type</span><span class="sxs-lookup"><span data-stu-id="e80e7-112">type</span></span>|[<span data-ttu-id="e80e7-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="e80e7-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="e80e7-114">Tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e80e7-114">Device type.</span></span> <span data-ttu-id="e80e7-115">Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e80e7-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e80e7-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e80e7-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="e80e7-117">String</span><span class="sxs-lookup"><span data-stu-id="e80e7-117">String</span></span>|<span data-ttu-id="e80e7-118">Versão mínima do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e80e7-118">Minimum OS version</span></span>|
|<span data-ttu-id="e80e7-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="e80e7-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="e80e7-120">String</span><span class="sxs-lookup"><span data-stu-id="e80e7-120">String</span></span>|<span data-ttu-id="e80e7-121">Versão de sistema operacional máxima</span><span class="sxs-lookup"><span data-stu-id="e80e7-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="e80e7-122">Relações</span><span class="sxs-lookup"><span data-stu-id="e80e7-122">Relationships</span></span>
<span data-ttu-id="e80e7-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e80e7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e80e7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e80e7-124">JSON Representation</span></span>
<span data-ttu-id="e80e7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e80e7-125">Here is a JSON representation of the resource.</span></span>
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




