---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 582d836ae2b9e701f640026d171046bf962eab92
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124111"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="cdad7-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cdad7-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="cdad7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdad7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdad7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdad7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdad7-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="cdad7-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="cdad7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cdad7-108">Methods</span></span>
|<span data-ttu-id="cdad7-109">Método</span><span class="sxs-lookup"><span data-stu-id="cdad7-109">Method</span></span>|<span data-ttu-id="cdad7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cdad7-110">Return Type</span></span>|<span data-ttu-id="cdad7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdad7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cdad7-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cdad7-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="cdad7-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cdad7-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="cdad7-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cdad7-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="cdad7-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cdad7-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="cdad7-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cdad7-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="cdad7-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cdad7-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cdad7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdad7-118">Properties</span></span>
|<span data-ttu-id="cdad7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdad7-119">Property</span></span>|<span data-ttu-id="cdad7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdad7-120">Type</span></span>|<span data-ttu-id="cdad7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdad7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdad7-122">id</span><span class="sxs-lookup"><span data-stu-id="cdad7-122">id</span></span>|<span data-ttu-id="cdad7-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdad7-123">String</span></span>|<span data-ttu-id="cdad7-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="cdad7-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="cdad7-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cdad7-125">enrolledDeviceCount</span></span>|<span data-ttu-id="cdad7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cdad7-126">Int32</span></span>|<span data-ttu-id="cdad7-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="cdad7-127">Total enrolled device count.</span></span> <span data-ttu-id="cdad7-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="cdad7-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="cdad7-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="cdad7-129">mdmEnrolledCount</span></span>|<span data-ttu-id="cdad7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cdad7-130">Int32</span></span>|<span data-ttu-id="cdad7-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="cdad7-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="cdad7-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cdad7-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="cdad7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cdad7-133">Int32</span></span>|<span data-ttu-id="cdad7-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="cdad7-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="cdad7-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="cdad7-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="cdad7-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="cdad7-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="cdad7-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cdad7-137">Device operating system summary.</span></span>|
|<span data-ttu-id="cdad7-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="cdad7-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="cdad7-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="cdad7-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="cdad7-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="cdad7-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="cdad7-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="cdad7-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="cdad7-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="cdad7-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="cdad7-143">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="cdad7-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="cdad7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdad7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="cdad7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdad7-145">DateTimeOffset</span></span>|<span data-ttu-id="cdad7-146">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cdad7-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdad7-147">Relações</span><span class="sxs-lookup"><span data-stu-id="cdad7-147">Relationships</span></span>
<span data-ttu-id="cdad7-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdad7-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdad7-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdad7-149">JSON Representation</span></span>
<span data-ttu-id="cdad7-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdad7-150">Here is a JSON representation of the resource.</span></span>
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
    "unknownCount": 1024,
    "androidDedicatedCount": 1024,
    "androidDeviceAdminCount": 1024,
    "androidFullyManagedCount": 1024,
    "androidWorkProfileCount": 1024,
    "androidCorporateWorkProfileCount": 1024,
    "configMgrDeviceCount": 1024
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



