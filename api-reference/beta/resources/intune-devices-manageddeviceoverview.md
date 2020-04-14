---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03e8d7086a2612428e56e81648d6a76e2d58afb2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443936"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="83475-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83475-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="83475-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83475-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83475-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83475-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83475-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83475-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83475-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="83475-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="83475-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="83475-108">Methods</span></span>
|<span data-ttu-id="83475-109">Método</span><span class="sxs-lookup"><span data-stu-id="83475-109">Method</span></span>|<span data-ttu-id="83475-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83475-110">Return Type</span></span>|<span data-ttu-id="83475-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83475-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83475-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83475-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="83475-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83475-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="83475-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="83475-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="83475-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83475-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="83475-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83475-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="83475-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="83475-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83475-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83475-118">Properties</span></span>
|<span data-ttu-id="83475-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83475-119">Property</span></span>|<span data-ttu-id="83475-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="83475-120">Type</span></span>|<span data-ttu-id="83475-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="83475-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83475-122">id</span><span class="sxs-lookup"><span data-stu-id="83475-122">id</span></span>|<span data-ttu-id="83475-123">String</span><span class="sxs-lookup"><span data-stu-id="83475-123">String</span></span>|<span data-ttu-id="83475-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="83475-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="83475-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83475-125">enrolledDeviceCount</span></span>|<span data-ttu-id="83475-126">Int32</span><span class="sxs-lookup"><span data-stu-id="83475-126">Int32</span></span>|<span data-ttu-id="83475-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="83475-127">Total enrolled device count.</span></span> <span data-ttu-id="83475-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="83475-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="83475-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="83475-129">mdmEnrolledCount</span></span>|<span data-ttu-id="83475-130">Int32</span><span class="sxs-lookup"><span data-stu-id="83475-130">Int32</span></span>|<span data-ttu-id="83475-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="83475-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="83475-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="83475-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="83475-133">Int32</span><span class="sxs-lookup"><span data-stu-id="83475-133">Int32</span></span>|<span data-ttu-id="83475-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="83475-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="83475-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="83475-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="83475-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="83475-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="83475-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83475-137">Device operating system summary.</span></span>|
|<span data-ttu-id="83475-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="83475-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="83475-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="83475-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="83475-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="83475-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="83475-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="83475-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="83475-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="83475-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="83475-143">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="83475-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="83475-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83475-144">lastModifiedDateTime</span></span>|<span data-ttu-id="83475-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83475-145">DateTimeOffset</span></span>|<span data-ttu-id="83475-146">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="83475-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="83475-147">Relações</span><span class="sxs-lookup"><span data-stu-id="83475-147">Relationships</span></span>
<span data-ttu-id="83475-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83475-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83475-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83475-149">JSON Representation</span></span>
<span data-ttu-id="83475-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83475-150">Here is a JSON representation of the resource.</span></span>
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



