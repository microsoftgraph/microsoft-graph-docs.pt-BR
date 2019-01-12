---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a5abdd3b5455272de7d1cf73044a1356d728dd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981193"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="ed60f-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ed60f-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="ed60f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed60f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed60f-105">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ed60f-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="ed60f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed60f-106">Methods</span></span>
|<span data-ttu-id="ed60f-107">Método</span><span class="sxs-lookup"><span data-stu-id="ed60f-107">Method</span></span>|<span data-ttu-id="ed60f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed60f-108">Return Type</span></span>|<span data-ttu-id="ed60f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed60f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed60f-110">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ed60f-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="ed60f-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ed60f-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ed60f-112">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ed60f-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="ed60f-113">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ed60f-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="ed60f-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ed60f-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ed60f-115">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ed60f-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed60f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed60f-116">Properties</span></span>
|<span data-ttu-id="ed60f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed60f-117">Property</span></span>|<span data-ttu-id="ed60f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed60f-118">Type</span></span>|<span data-ttu-id="ed60f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed60f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed60f-120">id</span><span class="sxs-lookup"><span data-stu-id="ed60f-120">id</span></span>|<span data-ttu-id="ed60f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed60f-121">String</span></span>|<span data-ttu-id="ed60f-122">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="ed60f-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="ed60f-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed60f-123">enrolledDeviceCount</span></span>|<span data-ttu-id="ed60f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ed60f-124">Int32</span></span>|<span data-ttu-id="ed60f-125">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="ed60f-125">Total enrolled device count.</span></span> <span data-ttu-id="ed60f-126">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="ed60f-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="ed60f-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="ed60f-127">mdmEnrolledCount</span></span>|<span data-ttu-id="ed60f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ed60f-128">Int32</span></span>|<span data-ttu-id="ed60f-129">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="ed60f-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="ed60f-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed60f-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="ed60f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed60f-131">Int32</span></span>|<span data-ttu-id="ed60f-132">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="ed60f-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="ed60f-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ed60f-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="ed60f-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ed60f-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="ed60f-135">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ed60f-135">Device operating system summary.</span></span>|
|<span data-ttu-id="ed60f-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed60f-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="ed60f-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed60f-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="ed60f-138">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="ed60f-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed60f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ed60f-139">Relationships</span></span>
<span data-ttu-id="ed60f-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed60f-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed60f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed60f-141">JSON Representation</span></span>
<span data-ttu-id="ed60f-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed60f-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```



