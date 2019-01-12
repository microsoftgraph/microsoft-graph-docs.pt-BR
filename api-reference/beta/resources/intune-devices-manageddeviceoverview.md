---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 091871ed88903f4fcb3a3ad8be86e7b997f173b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932508"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="7d25d-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7d25d-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="7d25d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d25d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d25d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d25d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d25d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7d25d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d25d-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="7d25d-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="7d25d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d25d-108">Methods</span></span>
|<span data-ttu-id="7d25d-109">Método</span><span class="sxs-lookup"><span data-stu-id="7d25d-109">Method</span></span>|<span data-ttu-id="7d25d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d25d-110">Return Type</span></span>|<span data-ttu-id="7d25d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d25d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7d25d-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7d25d-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="7d25d-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7d25d-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7d25d-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7d25d-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="7d25d-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7d25d-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="7d25d-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7d25d-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7d25d-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7d25d-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d25d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d25d-118">Properties</span></span>
|<span data-ttu-id="7d25d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d25d-119">Property</span></span>|<span data-ttu-id="7d25d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d25d-120">Type</span></span>|<span data-ttu-id="7d25d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d25d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d25d-122">id</span><span class="sxs-lookup"><span data-stu-id="7d25d-122">id</span></span>|<span data-ttu-id="7d25d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d25d-123">String</span></span>|<span data-ttu-id="7d25d-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="7d25d-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="7d25d-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d25d-125">enrolledDeviceCount</span></span>|<span data-ttu-id="7d25d-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7d25d-126">Int32</span></span>|<span data-ttu-id="7d25d-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="7d25d-127">Total enrolled device count.</span></span> <span data-ttu-id="7d25d-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="7d25d-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="7d25d-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="7d25d-129">mdmEnrolledCount</span></span>|<span data-ttu-id="7d25d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7d25d-130">Int32</span></span>|<span data-ttu-id="7d25d-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="7d25d-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="7d25d-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d25d-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="7d25d-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7d25d-133">Int32</span></span>|<span data-ttu-id="7d25d-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="7d25d-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="7d25d-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7d25d-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="7d25d-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7d25d-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="7d25d-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d25d-137">Device operating system summary.</span></span>|
|<span data-ttu-id="7d25d-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7d25d-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="7d25d-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7d25d-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="7d25d-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="7d25d-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="7d25d-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7d25d-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="7d25d-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7d25d-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="7d25d-143">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="7d25d-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="7d25d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d25d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="7d25d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d25d-145">DateTimeOffset</span></span>|<span data-ttu-id="7d25d-146">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7d25d-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d25d-147">Relações</span><span class="sxs-lookup"><span data-stu-id="7d25d-147">Relationships</span></span>
<span data-ttu-id="7d25d-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d25d-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d25d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d25d-149">JSON Representation</span></span>
<span data-ttu-id="7d25d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d25d-150">Here is a JSON representation of the resource.</span></span>
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





