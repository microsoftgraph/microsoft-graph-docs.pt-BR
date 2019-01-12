---
title: tipo de recurso de managedDeviceCleanupSettings
description: Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 334b561ffa19d4161553f761ce65b7da7d9dbcfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961894"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="28820-103">tipo de recurso de managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="28820-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="28820-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28820-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28820-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28820-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28820-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="28820-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28820-107">Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.</span><span class="sxs-lookup"><span data-stu-id="28820-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="28820-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28820-108">Properties</span></span>
|<span data-ttu-id="28820-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28820-109">Property</span></span>|<span data-ttu-id="28820-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="28820-110">Type</span></span>|<span data-ttu-id="28820-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28820-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28820-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="28820-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="28820-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28820-113">String</span></span>|<span data-ttu-id="28820-114">Número de dias quando o dispositivo não foi contatado Intune.</span><span class="sxs-lookup"><span data-stu-id="28820-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28820-115">Relações</span><span class="sxs-lookup"><span data-stu-id="28820-115">Relationships</span></span>
<span data-ttu-id="28820-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28820-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28820-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28820-117">JSON Representation</span></span>
<span data-ttu-id="28820-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28820-118">Here is a JSON representation of the resource.</span></span>
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





