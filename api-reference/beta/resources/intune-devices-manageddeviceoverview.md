---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07a6bda1e62088eabc3450cf2dcefc945f3ca898
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771198"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="96c41-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96c41-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="96c41-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96c41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96c41-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96c41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96c41-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="96c41-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="96c41-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="96c41-107">Methods</span></span>
|<span data-ttu-id="96c41-108">Método</span><span class="sxs-lookup"><span data-stu-id="96c41-108">Method</span></span>|<span data-ttu-id="96c41-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96c41-109">Return Type</span></span>|<span data-ttu-id="96c41-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c41-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="96c41-111">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96c41-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="96c41-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96c41-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="96c41-113">Ler propriedades e relações do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="96c41-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="96c41-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96c41-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="96c41-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="96c41-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="96c41-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="96c41-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="96c41-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96c41-117">Properties</span></span>
|<span data-ttu-id="96c41-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96c41-118">Property</span></span>|<span data-ttu-id="96c41-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="96c41-119">Type</span></span>|<span data-ttu-id="96c41-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c41-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96c41-121">id</span><span class="sxs-lookup"><span data-stu-id="96c41-121">id</span></span>|<span data-ttu-id="96c41-122">String</span><span class="sxs-lookup"><span data-stu-id="96c41-122">String</span></span>|<span data-ttu-id="96c41-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="96c41-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="96c41-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96c41-124">enrolledDeviceCount</span></span>|<span data-ttu-id="96c41-125">Int32</span><span class="sxs-lookup"><span data-stu-id="96c41-125">Int32</span></span>|<span data-ttu-id="96c41-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="96c41-126">Total enrolled device count.</span></span> <span data-ttu-id="96c41-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="96c41-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="96c41-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="96c41-128">mdmEnrolledCount</span></span>|<span data-ttu-id="96c41-129">Int32</span><span class="sxs-lookup"><span data-stu-id="96c41-129">Int32</span></span>|<span data-ttu-id="96c41-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="96c41-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="96c41-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="96c41-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="96c41-132">Int32</span><span class="sxs-lookup"><span data-stu-id="96c41-132">Int32</span></span>|<span data-ttu-id="96c41-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="96c41-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="96c41-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="96c41-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="96c41-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="96c41-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="96c41-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96c41-136">Device operating system summary.</span></span>|
|<span data-ttu-id="96c41-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="96c41-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="96c41-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="96c41-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="96c41-139">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="96c41-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="96c41-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="96c41-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="96c41-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="96c41-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="96c41-142">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="96c41-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="96c41-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96c41-143">lastModifiedDateTime</span></span>|<span data-ttu-id="96c41-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96c41-144">DateTimeOffset</span></span>|<span data-ttu-id="96c41-145">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="96c41-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="96c41-146">Relações</span><span class="sxs-lookup"><span data-stu-id="96c41-146">Relationships</span></span>
<span data-ttu-id="96c41-147">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="96c41-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96c41-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96c41-148">JSON Representation</span></span>
<span data-ttu-id="96c41-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96c41-149">Here is a JSON representation of the resource.</span></span>
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





