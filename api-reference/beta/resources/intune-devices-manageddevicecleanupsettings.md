---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86003dfd0121b6d4056377e8cf340497f41ccbd9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783960"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="1e09e-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="1e09e-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="1e09e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e09e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e09e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e09e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e09e-106">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="1e09e-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="1e09e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e09e-107">Properties</span></span>
|<span data-ttu-id="1e09e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e09e-108">Property</span></span>|<span data-ttu-id="1e09e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e09e-109">Type</span></span>|<span data-ttu-id="1e09e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e09e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e09e-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="1e09e-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="1e09e-112">String</span><span class="sxs-lookup"><span data-stu-id="1e09e-112">String</span></span>|<span data-ttu-id="1e09e-113">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="1e09e-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e09e-114">Relações</span><span class="sxs-lookup"><span data-stu-id="1e09e-114">Relationships</span></span>
<span data-ttu-id="1e09e-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e09e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e09e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e09e-116">JSON Representation</span></span>
<span data-ttu-id="1e09e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e09e-117">Here is a JSON representation of the resource.</span></span>
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



