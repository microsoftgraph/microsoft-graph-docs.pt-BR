---
title: tipo de recurso de managedDeviceCleanupSettings
description: Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.
ms.openlocfilehash: f7782ac9d6571b58c8ed1e7964637736fcb5f3d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037169"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="7019e-103">tipo de recurso de managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="7019e-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="7019e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7019e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7019e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7019e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7019e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7019e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7019e-107">Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.</span><span class="sxs-lookup"><span data-stu-id="7019e-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="7019e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7019e-108">Properties</span></span>
|<span data-ttu-id="7019e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7019e-109">Property</span></span>|<span data-ttu-id="7019e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7019e-110">Type</span></span>|<span data-ttu-id="7019e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7019e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7019e-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="7019e-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="7019e-113">String</span><span class="sxs-lookup"><span data-stu-id="7019e-113">String</span></span>|<span data-ttu-id="7019e-114">Número de dias quando o dispositivo não foi contatado Intune.</span><span class="sxs-lookup"><span data-stu-id="7019e-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7019e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="7019e-115">Relationships</span></span>
<span data-ttu-id="7019e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7019e-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7019e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7019e-117">JSON Representation</span></span>
<span data-ttu-id="7019e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7019e-118">Here is a JSON representation of the resource.</span></span>
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





