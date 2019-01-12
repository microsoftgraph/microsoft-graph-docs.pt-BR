---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fda8ac13e97f7c5dd6ed1efda0443b2f898c91c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959010"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="fcc74-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="fcc74-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="fcc74-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fcc74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcc74-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fcc74-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="fcc74-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcc74-106">Properties</span></span>
|<span data-ttu-id="fcc74-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcc74-107">Property</span></span>|<span data-ttu-id="fcc74-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcc74-108">Type</span></span>|<span data-ttu-id="fcc74-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcc74-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc74-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="fcc74-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="fcc74-111">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc74-111">Int32</span></span>|<span data-ttu-id="fcc74-112">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="fcc74-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="fcc74-113">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="fcc74-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="fcc74-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="fcc74-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="fcc74-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="fcc74-115">Boolean</span></span>|<span data-ttu-id="fcc74-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="fcc74-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="fcc74-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="fcc74-117">secureByDefault</span></span>|<span data-ttu-id="fcc74-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="fcc74-118">Boolean</span></span>|<span data-ttu-id="fcc74-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="fcc74-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcc74-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fcc74-120">Relationships</span></span>
<span data-ttu-id="fcc74-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fcc74-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fcc74-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcc74-122">JSON Representation</span></span>
<span data-ttu-id="fcc74-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fcc74-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



