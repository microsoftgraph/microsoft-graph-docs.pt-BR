---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36ab0a845450d803b3f0ac3fb0b9ea58cc4d3d3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250793"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="591e4-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="591e4-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="591e4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="591e4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="591e4-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="591e4-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="591e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="591e4-106">Properties</span></span>
|<span data-ttu-id="591e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="591e4-107">Property</span></span>|<span data-ttu-id="591e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="591e4-108">Type</span></span>|<span data-ttu-id="591e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="591e4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="591e4-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="591e4-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="591e4-111">Int32</span><span class="sxs-lookup"><span data-stu-id="591e4-111">Int32</span></span>|<span data-ttu-id="591e4-112">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="591e4-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="591e4-113">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="591e4-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="591e4-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="591e4-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="591e4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="591e4-115">Boolean</span></span>|<span data-ttu-id="591e4-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="591e4-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="591e4-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="591e4-117">secureByDefault</span></span>|<span data-ttu-id="591e4-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="591e4-118">Boolean</span></span>|<span data-ttu-id="591e4-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="591e4-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="591e4-120">Relações</span><span class="sxs-lookup"><span data-stu-id="591e4-120">Relationships</span></span>
<span data-ttu-id="591e4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="591e4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="591e4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="591e4-122">JSON Representation</span></span>
<span data-ttu-id="591e4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="591e4-123">Here is a JSON representation of the resource.</span></span>
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



