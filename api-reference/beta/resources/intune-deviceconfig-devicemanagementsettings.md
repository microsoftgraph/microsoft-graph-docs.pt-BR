---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e92c8e88ecf620b4731bd3694dfb97e252d042f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973024"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="bedab-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="bedab-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="bedab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bedab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bedab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bedab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bedab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bedab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bedab-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bedab-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bedab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bedab-108">Properties</span></span>
|<span data-ttu-id="bedab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bedab-109">Property</span></span>|<span data-ttu-id="bedab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bedab-110">Type</span></span>|<span data-ttu-id="bedab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bedab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bedab-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="bedab-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="bedab-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bedab-113">Int32</span></span>|<span data-ttu-id="bedab-114">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="bedab-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="bedab-115">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="bedab-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="bedab-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="bedab-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="bedab-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="bedab-117">Boolean</span></span>|<span data-ttu-id="bedab-118">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="bedab-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="bedab-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="bedab-119">secureByDefault</span></span>|<span data-ttu-id="bedab-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="bedab-120">Boolean</span></span>|<span data-ttu-id="bedab-121">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="bedab-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="bedab-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="bedab-122">enhancedJailBreak</span></span>|<span data-ttu-id="bedab-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="bedab-123">Boolean</span></span>|<span data-ttu-id="bedab-124">É o recurso habilitado ou não para maior detecção de jailbreak.</span><span class="sxs-lookup"><span data-stu-id="bedab-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="bedab-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="bedab-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="bedab-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bedab-126">Int32</span></span>|<span data-ttu-id="bedab-127">Quando o dispositivo não check-in do número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="bedab-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="bedab-128">Valores válidos 30 a 270</span><span class="sxs-lookup"><span data-stu-id="bedab-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="bedab-129">Relações</span><span class="sxs-lookup"><span data-stu-id="bedab-129">Relationships</span></span>
<span data-ttu-id="bedab-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bedab-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bedab-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bedab-131">JSON Representation</span></span>
<span data-ttu-id="bedab-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bedab-132">Here is a JSON representation of the resource.</span></span>
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
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





