---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f51b328adc39b7e9767c9ededd940e4f34b962c
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162481"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="71495-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71495-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="71495-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71495-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71495-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71495-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71495-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="71495-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="71495-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="71495-107">Methods</span></span>
|<span data-ttu-id="71495-108">Método</span><span class="sxs-lookup"><span data-stu-id="71495-108">Method</span></span>|<span data-ttu-id="71495-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71495-109">Return Type</span></span>|<span data-ttu-id="71495-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71495-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71495-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71495-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="71495-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71495-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="71495-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="71495-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="71495-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71495-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="71495-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="71495-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="71495-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="71495-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71495-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71495-117">Properties</span></span>
|<span data-ttu-id="71495-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71495-118">Property</span></span>|<span data-ttu-id="71495-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="71495-119">Type</span></span>|<span data-ttu-id="71495-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71495-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71495-121">id</span><span class="sxs-lookup"><span data-stu-id="71495-121">id</span></span>|<span data-ttu-id="71495-122">String</span><span class="sxs-lookup"><span data-stu-id="71495-122">String</span></span>|<span data-ttu-id="71495-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="71495-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="71495-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71495-124">enrolledDeviceCount</span></span>|<span data-ttu-id="71495-125">Int32</span><span class="sxs-lookup"><span data-stu-id="71495-125">Int32</span></span>|<span data-ttu-id="71495-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="71495-126">Total enrolled device count.</span></span> <span data-ttu-id="71495-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="71495-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="71495-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="71495-128">mdmEnrolledCount</span></span>|<span data-ttu-id="71495-129">Int32</span><span class="sxs-lookup"><span data-stu-id="71495-129">Int32</span></span>|<span data-ttu-id="71495-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="71495-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="71495-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="71495-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="71495-132">Int32</span><span class="sxs-lookup"><span data-stu-id="71495-132">Int32</span></span>|<span data-ttu-id="71495-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="71495-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="71495-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="71495-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="71495-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="71495-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="71495-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71495-136">Device operating system summary.</span></span>|
|<span data-ttu-id="71495-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="71495-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="71495-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="71495-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="71495-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="71495-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="71495-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="71495-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="71495-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="71495-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="71495-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="71495-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="71495-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71495-143">lastModifiedDateTime</span></span>|<span data-ttu-id="71495-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71495-144">DateTimeOffset</span></span>|<span data-ttu-id="71495-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="71495-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="71495-146">Relações</span><span class="sxs-lookup"><span data-stu-id="71495-146">Relationships</span></span>
<span data-ttu-id="71495-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71495-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71495-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71495-148">JSON Representation</span></span>
<span data-ttu-id="71495-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71495-149">Here is a JSON representation of the resource.</span></span>
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



