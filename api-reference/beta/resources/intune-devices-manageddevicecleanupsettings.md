---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d7e91d632860e47275cda158acf4d816c64e835
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522115"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="d9b22-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="d9b22-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="d9b22-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9b22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9b22-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9b22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b22-106">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="d9b22-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="d9b22-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9b22-107">Properties</span></span>
|<span data-ttu-id="d9b22-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9b22-108">Property</span></span>|<span data-ttu-id="d9b22-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b22-109">Type</span></span>|<span data-ttu-id="d9b22-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9b22-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="d9b22-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="d9b22-112">String</span><span class="sxs-lookup"><span data-stu-id="d9b22-112">String</span></span>|<span data-ttu-id="d9b22-113">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="d9b22-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9b22-114">Relações</span><span class="sxs-lookup"><span data-stu-id="d9b22-114">Relationships</span></span>
<span data-ttu-id="d9b22-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d9b22-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9b22-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9b22-116">JSON Representation</span></span>
<span data-ttu-id="d9b22-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9b22-117">Here is a JSON representation of the resource.</span></span>
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





