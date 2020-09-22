---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad931dc531cea8212309abca74e4dae6b6105cdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074990"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="6d3d1-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6d3d1-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="6d3d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d3d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d3d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d3d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d3d1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d3d1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6d3d1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d3d1-107">Properties</span></span>
|<span data-ttu-id="6d3d1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d3d1-108">Property</span></span>|<span data-ttu-id="6d3d1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d3d1-109">Type</span></span>|<span data-ttu-id="6d3d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d3d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d3d1-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="6d3d1-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="6d3d1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6d3d1-112">Int32</span></span>|<span data-ttu-id="6d3d1-113">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="6d3d1-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="6d3d1-114">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="6d3d1-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="6d3d1-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="6d3d1-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="6d3d1-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d3d1-116">Boolean</span></span>|<span data-ttu-id="6d3d1-117">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="6d3d1-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="6d3d1-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="6d3d1-118">secureByDefault</span></span>|<span data-ttu-id="6d3d1-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d3d1-119">Boolean</span></span>|<span data-ttu-id="6d3d1-120">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="6d3d1-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d3d1-121">Relações</span><span class="sxs-lookup"><span data-stu-id="6d3d1-121">Relationships</span></span>
<span data-ttu-id="6d3d1-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d3d1-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d3d1-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d3d1-123">JSON Representation</span></span>
<span data-ttu-id="6d3d1-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d3d1-124">Here is a JSON representation of the resource.</span></span>
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









