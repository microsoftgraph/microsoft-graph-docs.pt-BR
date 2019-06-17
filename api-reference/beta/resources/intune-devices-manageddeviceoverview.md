---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ed08262d9b98fc0a72641f0605d717e68f2ba08
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995109"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="27544-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27544-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="27544-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27544-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27544-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="27544-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="27544-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="27544-107">Methods</span></span>
|<span data-ttu-id="27544-108">Método</span><span class="sxs-lookup"><span data-stu-id="27544-108">Method</span></span>|<span data-ttu-id="27544-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27544-109">Return Type</span></span>|<span data-ttu-id="27544-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27544-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="27544-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27544-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="27544-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27544-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="27544-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="27544-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="27544-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27544-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="27544-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="27544-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="27544-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="27544-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="27544-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27544-117">Properties</span></span>
|<span data-ttu-id="27544-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27544-118">Property</span></span>|<span data-ttu-id="27544-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="27544-119">Type</span></span>|<span data-ttu-id="27544-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27544-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27544-121">id</span><span class="sxs-lookup"><span data-stu-id="27544-121">id</span></span>|<span data-ttu-id="27544-122">String</span><span class="sxs-lookup"><span data-stu-id="27544-122">String</span></span>|<span data-ttu-id="27544-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="27544-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="27544-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27544-124">enrolledDeviceCount</span></span>|<span data-ttu-id="27544-125">Int32</span><span class="sxs-lookup"><span data-stu-id="27544-125">Int32</span></span>|<span data-ttu-id="27544-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="27544-126">Total enrolled device count.</span></span> <span data-ttu-id="27544-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="27544-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="27544-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="27544-128">mdmEnrolledCount</span></span>|<span data-ttu-id="27544-129">Int32</span><span class="sxs-lookup"><span data-stu-id="27544-129">Int32</span></span>|<span data-ttu-id="27544-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="27544-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="27544-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="27544-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="27544-132">Int32</span><span class="sxs-lookup"><span data-stu-id="27544-132">Int32</span></span>|<span data-ttu-id="27544-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="27544-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="27544-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="27544-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="27544-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="27544-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="27544-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="27544-136">Device operating system summary.</span></span>|
|<span data-ttu-id="27544-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="27544-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="27544-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="27544-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="27544-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="27544-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="27544-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="27544-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="27544-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="27544-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="27544-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="27544-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="27544-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27544-143">lastModifiedDateTime</span></span>|<span data-ttu-id="27544-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27544-144">DateTimeOffset</span></span>|<span data-ttu-id="27544-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="27544-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="27544-146">Relações</span><span class="sxs-lookup"><span data-stu-id="27544-146">Relationships</span></span>
<span data-ttu-id="27544-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27544-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27544-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27544-148">JSON Representation</span></span>
<span data-ttu-id="27544-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27544-149">Here is a JSON representation of the resource.</span></span>
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





