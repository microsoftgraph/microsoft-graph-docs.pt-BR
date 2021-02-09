---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2a0345b19c2c2954b0bce231ca05d1bc2d2adcb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158489"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="6be40-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6be40-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="6be40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6be40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6be40-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6be40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6be40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be40-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="6be40-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="6be40-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6be40-108">Methods</span></span>
|<span data-ttu-id="6be40-109">Método</span><span class="sxs-lookup"><span data-stu-id="6be40-109">Method</span></span>|<span data-ttu-id="6be40-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6be40-110">Return Type</span></span>|<span data-ttu-id="6be40-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6be40-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6be40-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6be40-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="6be40-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6be40-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="6be40-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="6be40-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="6be40-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6be40-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="6be40-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6be40-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="6be40-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="6be40-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6be40-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6be40-118">Properties</span></span>
|<span data-ttu-id="6be40-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6be40-119">Property</span></span>|<span data-ttu-id="6be40-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6be40-120">Type</span></span>|<span data-ttu-id="6be40-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6be40-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be40-122">id</span><span class="sxs-lookup"><span data-stu-id="6be40-122">id</span></span>|<span data-ttu-id="6be40-123">String</span><span class="sxs-lookup"><span data-stu-id="6be40-123">String</span></span>|<span data-ttu-id="6be40-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="6be40-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="6be40-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be40-125">enrolledDeviceCount</span></span>|<span data-ttu-id="6be40-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6be40-126">Int32</span></span>|<span data-ttu-id="6be40-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="6be40-127">Total enrolled device count.</span></span> <span data-ttu-id="6be40-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="6be40-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="6be40-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="6be40-129">mdmEnrolledCount</span></span>|<span data-ttu-id="6be40-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6be40-130">Int32</span></span>|<span data-ttu-id="6be40-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="6be40-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="6be40-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6be40-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="6be40-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6be40-133">Int32</span></span>|<span data-ttu-id="6be40-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="6be40-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="6be40-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6be40-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="6be40-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="6be40-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="6be40-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6be40-137">Device operating system summary.</span></span>|
|<span data-ttu-id="6be40-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6be40-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="6be40-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="6be40-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="6be40-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="6be40-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="6be40-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="6be40-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="6be40-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="6be40-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="6be40-143">Models and Manufactures manufactureadata for managed devices in the account</span><span class="sxs-lookup"><span data-stu-id="6be40-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="6be40-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6be40-144">lastModifiedDateTime</span></span>|<span data-ttu-id="6be40-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6be40-145">DateTimeOffset</span></span>|<span data-ttu-id="6be40-146">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6be40-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6be40-147">Relações</span><span class="sxs-lookup"><span data-stu-id="6be40-147">Relationships</span></span>
<span data-ttu-id="6be40-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6be40-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6be40-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6be40-149">JSON Representation</span></span>
<span data-ttu-id="6be40-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6be40-150">Here is a JSON representation of the resource.</span></span>
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
    "configMgrDeviceCount": 1024,
    "aospUserlessCount": 1024,
    "aospUserAssociatedCount": 1024
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




