---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1eeb349e8ec77adce3d69df9d61f43e43fb3b770
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872545"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="c1063-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c1063-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="c1063-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1063-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1063-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1063-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1063-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c1063-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1063-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="c1063-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="c1063-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1063-108">Methods</span></span>
|<span data-ttu-id="c1063-109">Método</span><span class="sxs-lookup"><span data-stu-id="c1063-109">Method</span></span>|<span data-ttu-id="c1063-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1063-110">Return Type</span></span>|<span data-ttu-id="c1063-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1063-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c1063-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c1063-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="c1063-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c1063-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c1063-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c1063-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="c1063-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c1063-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="c1063-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c1063-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c1063-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c1063-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1063-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1063-118">Properties</span></span>
|<span data-ttu-id="c1063-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1063-119">Property</span></span>|<span data-ttu-id="c1063-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1063-120">Type</span></span>|<span data-ttu-id="c1063-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1063-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1063-122">id</span><span class="sxs-lookup"><span data-stu-id="c1063-122">id</span></span>|<span data-ttu-id="c1063-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1063-123">String</span></span>|<span data-ttu-id="c1063-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="c1063-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="c1063-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1063-125">enrolledDeviceCount</span></span>|<span data-ttu-id="c1063-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c1063-126">Int32</span></span>|<span data-ttu-id="c1063-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="c1063-127">Total enrolled device count.</span></span> <span data-ttu-id="c1063-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="c1063-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="c1063-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="c1063-129">mdmEnrolledCount</span></span>|<span data-ttu-id="c1063-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c1063-130">Int32</span></span>|<span data-ttu-id="c1063-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="c1063-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="c1063-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c1063-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="c1063-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c1063-133">Int32</span></span>|<span data-ttu-id="c1063-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="c1063-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="c1063-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c1063-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="c1063-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c1063-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="c1063-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1063-137">Device operating system summary.</span></span>|
|<span data-ttu-id="c1063-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c1063-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="c1063-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c1063-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="c1063-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="c1063-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="c1063-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c1063-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="c1063-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c1063-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="c1063-143">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="c1063-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="c1063-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1063-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c1063-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1063-145">DateTimeOffset</span></span>|<span data-ttu-id="c1063-146">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c1063-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1063-147">Relações</span><span class="sxs-lookup"><span data-stu-id="c1063-147">Relationships</span></span>
<span data-ttu-id="c1063-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1063-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1063-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1063-149">JSON Representation</span></span>
<span data-ttu-id="c1063-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1063-150">Here is a JSON representation of the resource.</span></span>
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





