---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7deb73e1fa9557e212d8fab524f62f15bad4b249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867253"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="985e5-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="985e5-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="985e5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="985e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="985e5-105">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="985e5-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="985e5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="985e5-106">Methods</span></span>
|<span data-ttu-id="985e5-107">Método</span><span class="sxs-lookup"><span data-stu-id="985e5-107">Method</span></span>|<span data-ttu-id="985e5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="985e5-108">Return Type</span></span>|<span data-ttu-id="985e5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="985e5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="985e5-110">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="985e5-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="985e5-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="985e5-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="985e5-112">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="985e5-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="985e5-113">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="985e5-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="985e5-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="985e5-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="985e5-115">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="985e5-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="985e5-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="985e5-116">Properties</span></span>
|<span data-ttu-id="985e5-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="985e5-117">Property</span></span>|<span data-ttu-id="985e5-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="985e5-118">Type</span></span>|<span data-ttu-id="985e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="985e5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="985e5-120">id</span><span class="sxs-lookup"><span data-stu-id="985e5-120">id</span></span>|<span data-ttu-id="985e5-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="985e5-121">String</span></span>|<span data-ttu-id="985e5-122">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="985e5-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="985e5-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="985e5-123">enrolledDeviceCount</span></span>|<span data-ttu-id="985e5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="985e5-124">Int32</span></span>|<span data-ttu-id="985e5-125">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="985e5-125">Total enrolled device count.</span></span> <span data-ttu-id="985e5-126">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="985e5-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="985e5-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="985e5-127">mdmEnrolledCount</span></span>|<span data-ttu-id="985e5-128">Int32</span><span class="sxs-lookup"><span data-stu-id="985e5-128">Int32</span></span>|<span data-ttu-id="985e5-129">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="985e5-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="985e5-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="985e5-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="985e5-131">Int32</span><span class="sxs-lookup"><span data-stu-id="985e5-131">Int32</span></span>|<span data-ttu-id="985e5-132">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="985e5-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="985e5-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="985e5-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="985e5-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="985e5-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="985e5-135">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="985e5-135">Device operating system summary.</span></span>|
|<span data-ttu-id="985e5-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="985e5-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="985e5-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="985e5-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="985e5-138">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="985e5-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="985e5-139">Relações</span><span class="sxs-lookup"><span data-stu-id="985e5-139">Relationships</span></span>
<span data-ttu-id="985e5-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="985e5-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="985e5-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="985e5-141">JSON Representation</span></span>
<span data-ttu-id="985e5-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="985e5-142">Here is a JSON representation of the resource.</span></span>
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



