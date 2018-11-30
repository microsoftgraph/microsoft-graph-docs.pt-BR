---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
ms.openlocfilehash: 11f1012329d0217499d813b94f72474da8c683a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037183"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="920ee-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="920ee-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="920ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="920ee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="920ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="920ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="920ee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="920ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="920ee-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="920ee-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="920ee-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="920ee-108">Methods</span></span>
|<span data-ttu-id="920ee-109">Método</span><span class="sxs-lookup"><span data-stu-id="920ee-109">Method</span></span>|<span data-ttu-id="920ee-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="920ee-110">Return Type</span></span>|<span data-ttu-id="920ee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="920ee-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="920ee-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="920ee-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="920ee-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="920ee-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="920ee-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="920ee-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="920ee-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="920ee-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="920ee-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="920ee-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="920ee-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="920ee-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="920ee-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="920ee-118">Properties</span></span>
|<span data-ttu-id="920ee-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="920ee-119">Property</span></span>|<span data-ttu-id="920ee-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="920ee-120">Type</span></span>|<span data-ttu-id="920ee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="920ee-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="920ee-122">id</span><span class="sxs-lookup"><span data-stu-id="920ee-122">id</span></span>|<span data-ttu-id="920ee-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="920ee-123">String</span></span>|<span data-ttu-id="920ee-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="920ee-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="920ee-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="920ee-125">enrolledDeviceCount</span></span>|<span data-ttu-id="920ee-126">Int32</span><span class="sxs-lookup"><span data-stu-id="920ee-126">Int32</span></span>|<span data-ttu-id="920ee-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="920ee-127">Total enrolled device count.</span></span> <span data-ttu-id="920ee-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="920ee-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="920ee-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="920ee-129">mdmEnrolledCount</span></span>|<span data-ttu-id="920ee-130">Int32</span><span class="sxs-lookup"><span data-stu-id="920ee-130">Int32</span></span>|<span data-ttu-id="920ee-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="920ee-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="920ee-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="920ee-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="920ee-133">Int32</span><span class="sxs-lookup"><span data-stu-id="920ee-133">Int32</span></span>|<span data-ttu-id="920ee-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="920ee-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="920ee-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="920ee-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="920ee-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="920ee-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="920ee-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="920ee-137">Device operating system summary.</span></span>|
|<span data-ttu-id="920ee-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="920ee-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="920ee-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="920ee-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="920ee-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="920ee-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="920ee-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="920ee-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="920ee-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="920ee-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="920ee-143">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="920ee-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="920ee-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="920ee-144">lastModifiedDateTime</span></span>|<span data-ttu-id="920ee-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="920ee-145">DateTimeOffset</span></span>|<span data-ttu-id="920ee-146">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="920ee-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="920ee-147">Relações</span><span class="sxs-lookup"><span data-stu-id="920ee-147">Relationships</span></span>
<span data-ttu-id="920ee-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="920ee-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="920ee-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="920ee-149">JSON Representation</span></span>
<span data-ttu-id="920ee-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="920ee-150">Here is a JSON representation of the resource.</span></span>
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





