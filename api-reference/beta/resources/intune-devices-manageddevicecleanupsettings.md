---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e37b45c61bdc96b47b0b8ca29dd5bc44689addc9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443958"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="db649-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="db649-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="db649-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db649-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db649-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db649-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db649-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db649-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db649-107">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="db649-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="db649-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db649-108">Properties</span></span>
|<span data-ttu-id="db649-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db649-109">Property</span></span>|<span data-ttu-id="db649-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="db649-110">Type</span></span>|<span data-ttu-id="db649-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="db649-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db649-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="db649-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="db649-113">String</span><span class="sxs-lookup"><span data-stu-id="db649-113">String</span></span>|<span data-ttu-id="db649-114">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="db649-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db649-115">Relações</span><span class="sxs-lookup"><span data-stu-id="db649-115">Relationships</span></span>
<span data-ttu-id="db649-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db649-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db649-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db649-117">JSON Representation</span></span>
<span data-ttu-id="db649-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db649-118">Here is a JSON representation of the resource.</span></span>
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



