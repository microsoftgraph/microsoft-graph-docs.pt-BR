---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 686482077d201f952d73af46519650122d60e8b9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091121"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="55824-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55824-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="55824-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55824-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55824-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55824-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55824-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="55824-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="55824-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="55824-107">Methods</span></span>
|<span data-ttu-id="55824-108">Método</span><span class="sxs-lookup"><span data-stu-id="55824-108">Method</span></span>|<span data-ttu-id="55824-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55824-109">Return Type</span></span>|<span data-ttu-id="55824-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55824-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55824-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55824-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="55824-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55824-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="55824-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55824-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="55824-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55824-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="55824-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55824-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="55824-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55824-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55824-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55824-117">Properties</span></span>
|<span data-ttu-id="55824-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55824-118">Property</span></span>|<span data-ttu-id="55824-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="55824-119">Type</span></span>|<span data-ttu-id="55824-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="55824-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55824-121">id</span><span class="sxs-lookup"><span data-stu-id="55824-121">id</span></span>|<span data-ttu-id="55824-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55824-122">String</span></span>|<span data-ttu-id="55824-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="55824-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="55824-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55824-124">enrolledDeviceCount</span></span>|<span data-ttu-id="55824-125">Int32</span><span class="sxs-lookup"><span data-stu-id="55824-125">Int32</span></span>|<span data-ttu-id="55824-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="55824-126">Total enrolled device count.</span></span> <span data-ttu-id="55824-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="55824-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="55824-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="55824-128">mdmEnrolledCount</span></span>|<span data-ttu-id="55824-129">Int32</span><span class="sxs-lookup"><span data-stu-id="55824-129">Int32</span></span>|<span data-ttu-id="55824-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="55824-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="55824-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55824-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="55824-132">Int32</span><span class="sxs-lookup"><span data-stu-id="55824-132">Int32</span></span>|<span data-ttu-id="55824-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="55824-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="55824-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="55824-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="55824-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="55824-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="55824-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55824-136">Device operating system summary.</span></span>|
|<span data-ttu-id="55824-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="55824-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="55824-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="55824-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="55824-139">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="55824-139">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="55824-140">Relações</span><span class="sxs-lookup"><span data-stu-id="55824-140">Relationships</span></span>
<span data-ttu-id="55824-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55824-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55824-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55824-142">JSON Representation</span></span>
<span data-ttu-id="55824-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55824-143">Here is a JSON representation of the resource.</span></span>
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
  }
}
```









