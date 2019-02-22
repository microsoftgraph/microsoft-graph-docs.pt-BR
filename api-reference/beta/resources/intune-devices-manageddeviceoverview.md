---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6c7187bc5cb984e4ca7e607068e6010f747f868
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175000"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="69fa6-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="69fa6-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="69fa6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69fa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69fa6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69fa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69fa6-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="69fa6-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="69fa6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="69fa6-107">Methods</span></span>
|<span data-ttu-id="69fa6-108">Método</span><span class="sxs-lookup"><span data-stu-id="69fa6-108">Method</span></span>|<span data-ttu-id="69fa6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69fa6-109">Return Type</span></span>|<span data-ttu-id="69fa6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="69fa6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69fa6-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="69fa6-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="69fa6-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="69fa6-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="69fa6-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="69fa6-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="69fa6-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="69fa6-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="69fa6-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="69fa6-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="69fa6-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="69fa6-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69fa6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69fa6-117">Properties</span></span>
|<span data-ttu-id="69fa6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69fa6-118">Property</span></span>|<span data-ttu-id="69fa6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="69fa6-119">Type</span></span>|<span data-ttu-id="69fa6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69fa6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69fa6-121">id</span><span class="sxs-lookup"><span data-stu-id="69fa6-121">id</span></span>|<span data-ttu-id="69fa6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69fa6-122">String</span></span>|<span data-ttu-id="69fa6-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="69fa6-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="69fa6-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69fa6-124">enrolledDeviceCount</span></span>|<span data-ttu-id="69fa6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="69fa6-125">Int32</span></span>|<span data-ttu-id="69fa6-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="69fa6-126">Total enrolled device count.</span></span> <span data-ttu-id="69fa6-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="69fa6-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="69fa6-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="69fa6-128">mdmEnrolledCount</span></span>|<span data-ttu-id="69fa6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="69fa6-129">Int32</span></span>|<span data-ttu-id="69fa6-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="69fa6-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="69fa6-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69fa6-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="69fa6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="69fa6-132">Int32</span></span>|<span data-ttu-id="69fa6-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="69fa6-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="69fa6-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="69fa6-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="69fa6-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="69fa6-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="69fa6-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="69fa6-136">Device operating system summary.</span></span>|
|<span data-ttu-id="69fa6-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="69fa6-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="69fa6-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="69fa6-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="69fa6-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="69fa6-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="69fa6-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="69fa6-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="69fa6-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="69fa6-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="69fa6-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="69fa6-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="69fa6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69fa6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="69fa6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69fa6-144">DateTimeOffset</span></span>|<span data-ttu-id="69fa6-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="69fa6-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="69fa6-146">Relações</span><span class="sxs-lookup"><span data-stu-id="69fa6-146">Relationships</span></span>
<span data-ttu-id="69fa6-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69fa6-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69fa6-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69fa6-148">JSON Representation</span></span>
<span data-ttu-id="69fa6-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69fa6-149">Here is a JSON representation of the resource.</span></span>
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```




