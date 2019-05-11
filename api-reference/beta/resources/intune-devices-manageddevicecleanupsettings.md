---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5070de01324b25332d42b63a4d1d787989b86c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941958"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="c5f20-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="c5f20-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="c5f20-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5f20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5f20-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5f20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5f20-106">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="c5f20-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="c5f20-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5f20-107">Properties</span></span>
|<span data-ttu-id="c5f20-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5f20-108">Property</span></span>|<span data-ttu-id="c5f20-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f20-109">Type</span></span>|<span data-ttu-id="c5f20-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5f20-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="c5f20-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="c5f20-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f20-112">String</span></span>|<span data-ttu-id="c5f20-113">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="c5f20-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5f20-114">Relações</span><span class="sxs-lookup"><span data-stu-id="c5f20-114">Relationships</span></span>
<span data-ttu-id="c5f20-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5f20-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5f20-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5f20-116">JSON Representation</span></span>
<span data-ttu-id="c5f20-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5f20-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```




