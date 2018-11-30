---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
ms.openlocfilehash: 4a07c879e20139c9138fc7315172655aa48a40eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004776"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="8eebe-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="8eebe-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="8eebe-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8eebe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8eebe-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8eebe-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8eebe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eebe-106">Properties</span></span>
|<span data-ttu-id="8eebe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eebe-107">Property</span></span>|<span data-ttu-id="8eebe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eebe-108">Type</span></span>|<span data-ttu-id="8eebe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eebe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eebe-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="8eebe-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="8eebe-111">Int32</span><span class="sxs-lookup"><span data-stu-id="8eebe-111">Int32</span></span>|<span data-ttu-id="8eebe-112">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="8eebe-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="8eebe-113">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="8eebe-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="8eebe-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="8eebe-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="8eebe-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eebe-115">Boolean</span></span>|<span data-ttu-id="8eebe-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="8eebe-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="8eebe-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="8eebe-117">secureByDefault</span></span>|<span data-ttu-id="8eebe-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eebe-118">Boolean</span></span>|<span data-ttu-id="8eebe-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="8eebe-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eebe-120">Relações</span><span class="sxs-lookup"><span data-stu-id="8eebe-120">Relationships</span></span>
<span data-ttu-id="8eebe-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8eebe-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8eebe-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eebe-122">JSON Representation</span></span>
<span data-ttu-id="8eebe-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eebe-123">Here is a JSON representation of the resource.</span></span>
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



