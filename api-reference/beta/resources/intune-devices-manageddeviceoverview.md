---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db5cebe36850971c871f673d07f18b8d5121cb1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422233"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="38a79-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38a79-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="38a79-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="38a79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38a79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38a79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38a79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="38a79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a79-107">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="38a79-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="38a79-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="38a79-108">Methods</span></span>
|<span data-ttu-id="38a79-109">Método</span><span class="sxs-lookup"><span data-stu-id="38a79-109">Method</span></span>|<span data-ttu-id="38a79-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38a79-110">Return Type</span></span>|<span data-ttu-id="38a79-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a79-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38a79-112">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38a79-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="38a79-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38a79-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="38a79-114">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="38a79-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="38a79-115">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38a79-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="38a79-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="38a79-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="38a79-117">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="38a79-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38a79-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38a79-118">Properties</span></span>
|<span data-ttu-id="38a79-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38a79-119">Property</span></span>|<span data-ttu-id="38a79-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a79-120">Type</span></span>|<span data-ttu-id="38a79-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a79-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a79-122">id</span><span class="sxs-lookup"><span data-stu-id="38a79-122">id</span></span>|<span data-ttu-id="38a79-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38a79-123">String</span></span>|<span data-ttu-id="38a79-124">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="38a79-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="38a79-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="38a79-125">enrolledDeviceCount</span></span>|<span data-ttu-id="38a79-126">Int32</span><span class="sxs-lookup"><span data-stu-id="38a79-126">Int32</span></span>|<span data-ttu-id="38a79-127">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="38a79-127">Total enrolled device count.</span></span> <span data-ttu-id="38a79-128">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="38a79-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="38a79-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="38a79-129">mdmEnrolledCount</span></span>|<span data-ttu-id="38a79-130">Int32</span><span class="sxs-lookup"><span data-stu-id="38a79-130">Int32</span></span>|<span data-ttu-id="38a79-131">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="38a79-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="38a79-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="38a79-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="38a79-133">Int32</span><span class="sxs-lookup"><span data-stu-id="38a79-133">Int32</span></span>|<span data-ttu-id="38a79-134">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="38a79-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="38a79-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="38a79-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="38a79-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="38a79-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="38a79-137">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38a79-137">Device operating system summary.</span></span>|
|<span data-ttu-id="38a79-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="38a79-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="38a79-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="38a79-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="38a79-140">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="38a79-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="38a79-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="38a79-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="38a79-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="38a79-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="38a79-143">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="38a79-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="38a79-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38a79-144">lastModifiedDateTime</span></span>|<span data-ttu-id="38a79-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a79-145">DateTimeOffset</span></span>|<span data-ttu-id="38a79-146">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="38a79-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a79-147">Relações</span><span class="sxs-lookup"><span data-stu-id="38a79-147">Relationships</span></span>
<span data-ttu-id="38a79-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38a79-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38a79-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38a79-149">JSON Representation</span></span>
<span data-ttu-id="38a79-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38a79-150">Here is a JSON representation of the resource.</span></span>
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




