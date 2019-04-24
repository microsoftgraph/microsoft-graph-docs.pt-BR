---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36ab0a845450d803b3f0ac3fb0b9ea58cc4d3d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460930"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="55e70-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="55e70-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="55e70-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55e70-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55e70-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="55e70-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="55e70-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55e70-106">Properties</span></span>
|<span data-ttu-id="55e70-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55e70-107">Property</span></span>|<span data-ttu-id="55e70-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="55e70-108">Type</span></span>|<span data-ttu-id="55e70-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55e70-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55e70-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="55e70-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="55e70-111">Int32</span><span class="sxs-lookup"><span data-stu-id="55e70-111">Int32</span></span>|<span data-ttu-id="55e70-112">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="55e70-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="55e70-113">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="55e70-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="55e70-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="55e70-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="55e70-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="55e70-115">Boolean</span></span>|<span data-ttu-id="55e70-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="55e70-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="55e70-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="55e70-117">secureByDefault</span></span>|<span data-ttu-id="55e70-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="55e70-118">Boolean</span></span>|<span data-ttu-id="55e70-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="55e70-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="55e70-120">Relações</span><span class="sxs-lookup"><span data-stu-id="55e70-120">Relationships</span></span>
<span data-ttu-id="55e70-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="55e70-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55e70-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55e70-122">JSON Representation</span></span>
<span data-ttu-id="55e70-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55e70-123">Here is a JSON representation of the resource.</span></span>
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



