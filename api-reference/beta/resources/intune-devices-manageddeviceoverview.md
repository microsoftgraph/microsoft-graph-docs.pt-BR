---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bff057f872a8b315e0335f5d68633fce6d04e71
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783946"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="ebb53-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebb53-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="ebb53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebb53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebb53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb53-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ebb53-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="ebb53-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebb53-107">Methods</span></span>
|<span data-ttu-id="ebb53-108">Método</span><span class="sxs-lookup"><span data-stu-id="ebb53-108">Method</span></span>|<span data-ttu-id="ebb53-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebb53-109">Return Type</span></span>|<span data-ttu-id="ebb53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebb53-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebb53-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebb53-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="ebb53-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebb53-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ebb53-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ebb53-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="ebb53-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebb53-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="ebb53-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ebb53-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ebb53-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ebb53-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebb53-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebb53-117">Properties</span></span>
|<span data-ttu-id="ebb53-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebb53-118">Property</span></span>|<span data-ttu-id="ebb53-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebb53-119">Type</span></span>|<span data-ttu-id="ebb53-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebb53-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb53-121">id</span><span class="sxs-lookup"><span data-stu-id="ebb53-121">id</span></span>|<span data-ttu-id="ebb53-122">String</span><span class="sxs-lookup"><span data-stu-id="ebb53-122">String</span></span>|<span data-ttu-id="ebb53-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="ebb53-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="ebb53-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebb53-124">enrolledDeviceCount</span></span>|<span data-ttu-id="ebb53-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb53-125">Int32</span></span>|<span data-ttu-id="ebb53-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="ebb53-126">Total enrolled device count.</span></span> <span data-ttu-id="ebb53-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="ebb53-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="ebb53-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="ebb53-128">mdmEnrolledCount</span></span>|<span data-ttu-id="ebb53-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb53-129">Int32</span></span>|<span data-ttu-id="ebb53-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="ebb53-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="ebb53-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebb53-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="ebb53-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb53-132">Int32</span></span>|<span data-ttu-id="ebb53-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="ebb53-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="ebb53-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ebb53-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="ebb53-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ebb53-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="ebb53-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebb53-136">Device operating system summary.</span></span>|
|<span data-ttu-id="ebb53-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ebb53-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="ebb53-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ebb53-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="ebb53-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="ebb53-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="ebb53-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="ebb53-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="ebb53-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="ebb53-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="ebb53-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="ebb53-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="ebb53-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb53-143">lastModifiedDateTime</span></span>|<span data-ttu-id="ebb53-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb53-144">DateTimeOffset</span></span>|<span data-ttu-id="ebb53-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ebb53-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebb53-146">Relações</span><span class="sxs-lookup"><span data-stu-id="ebb53-146">Relationships</span></span>
<span data-ttu-id="ebb53-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebb53-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb53-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebb53-148">JSON Representation</span></span>
<span data-ttu-id="ebb53-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebb53-149">Here is a JSON representation of the resource.</span></span>
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



