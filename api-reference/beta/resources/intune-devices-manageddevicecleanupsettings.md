---
title: tipo de recurso de managedDeviceCleanupSettings
description: Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.
author: tfitzmac
ms.openlocfilehash: 84650c4d2d182fe0da30ced56786a2c0216a6358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304085"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="e5f0a-103">tipo de recurso de managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="e5f0a-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="e5f0a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5f0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5f0a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5f0a-107">Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="e5f0a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5f0a-108">Properties</span></span>
|<span data-ttu-id="e5f0a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5f0a-109">Property</span></span>|<span data-ttu-id="e5f0a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5f0a-110">Type</span></span>|<span data-ttu-id="e5f0a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5f0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5f0a-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="e5f0a-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="e5f0a-113">String</span><span class="sxs-lookup"><span data-stu-id="e5f0a-113">String</span></span>|<span data-ttu-id="e5f0a-114">Número de dias quando o dispositivo não foi contatado Intune.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5f0a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e5f0a-115">Relationships</span></span>
<span data-ttu-id="e5f0a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5f0a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5f0a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5f0a-117">JSON Representation</span></span>
<span data-ttu-id="e5f0a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5f0a-118">Here is a JSON representation of the resource.</span></span>
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





