---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e076e1e32f72ec352984c92076a33e57005cce6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999742"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="47e63-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47e63-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="47e63-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47e63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47e63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47e63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e63-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="47e63-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="47e63-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="47e63-107">Methods</span></span>
|<span data-ttu-id="47e63-108">Método</span><span class="sxs-lookup"><span data-stu-id="47e63-108">Method</span></span>|<span data-ttu-id="47e63-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="47e63-109">Return Type</span></span>|<span data-ttu-id="47e63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e63-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47e63-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47e63-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="47e63-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47e63-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="47e63-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="47e63-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="47e63-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47e63-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="47e63-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="47e63-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="47e63-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="47e63-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47e63-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47e63-117">Properties</span></span>
|<span data-ttu-id="47e63-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47e63-118">Property</span></span>|<span data-ttu-id="47e63-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="47e63-119">Type</span></span>|<span data-ttu-id="47e63-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47e63-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e63-121">id</span><span class="sxs-lookup"><span data-stu-id="47e63-121">id</span></span>|<span data-ttu-id="47e63-122">String</span><span class="sxs-lookup"><span data-stu-id="47e63-122">String</span></span>|<span data-ttu-id="47e63-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="47e63-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="47e63-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47e63-124">enrolledDeviceCount</span></span>|<span data-ttu-id="47e63-125">Int32</span><span class="sxs-lookup"><span data-stu-id="47e63-125">Int32</span></span>|<span data-ttu-id="47e63-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="47e63-126">Total enrolled device count.</span></span> <span data-ttu-id="47e63-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="47e63-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="47e63-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="47e63-128">mdmEnrolledCount</span></span>|<span data-ttu-id="47e63-129">Int32</span><span class="sxs-lookup"><span data-stu-id="47e63-129">Int32</span></span>|<span data-ttu-id="47e63-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="47e63-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="47e63-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="47e63-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="47e63-132">Int32</span><span class="sxs-lookup"><span data-stu-id="47e63-132">Int32</span></span>|<span data-ttu-id="47e63-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="47e63-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="47e63-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="47e63-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="47e63-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="47e63-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="47e63-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47e63-136">Device operating system summary.</span></span>|
|<span data-ttu-id="47e63-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="47e63-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="47e63-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="47e63-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="47e63-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="47e63-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="47e63-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="47e63-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="47e63-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="47e63-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="47e63-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="47e63-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="47e63-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47e63-143">lastModifiedDateTime</span></span>|<span data-ttu-id="47e63-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47e63-144">DateTimeOffset</span></span>|<span data-ttu-id="47e63-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="47e63-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="47e63-146">Relações</span><span class="sxs-lookup"><span data-stu-id="47e63-146">Relationships</span></span>
<span data-ttu-id="47e63-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47e63-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47e63-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47e63-148">JSON Representation</span></span>
<span data-ttu-id="47e63-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47e63-149">Here is a JSON representation of the resource.</span></span>
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





