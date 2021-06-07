---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17856c01f006206298e1efa1ed01fdcac6045557
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755095"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="a86f0-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="a86f0-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="a86f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a86f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a86f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a86f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a86f0-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a86f0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a86f0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a86f0-107">Properties</span></span>
|<span data-ttu-id="a86f0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a86f0-108">Property</span></span>|<span data-ttu-id="a86f0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a86f0-109">Type</span></span>|<span data-ttu-id="a86f0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a86f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a86f0-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a86f0-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="a86f0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a86f0-112">Int32</span></span>|<span data-ttu-id="a86f0-113">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a86f0-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="a86f0-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="a86f0-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="a86f0-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="a86f0-115">Boolean</span></span>|<span data-ttu-id="a86f0-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="a86f0-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="a86f0-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="a86f0-117">secureByDefault</span></span>|<span data-ttu-id="a86f0-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="a86f0-118">Boolean</span></span>|<span data-ttu-id="a86f0-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="a86f0-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="a86f0-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a86f0-120">Relationships</span></span>
<span data-ttu-id="a86f0-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a86f0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a86f0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a86f0-122">JSON Representation</span></span>
<span data-ttu-id="a86f0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a86f0-123">Here is a JSON representation of the resource.</span></span>
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




