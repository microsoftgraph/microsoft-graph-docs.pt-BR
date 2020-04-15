---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d0eb038d8bbc6291c7007184cdbde4e97656099
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406915"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b3bc8-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b3bc8-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="b3bc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3bc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3bc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3bc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3bc8-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="b3bc8-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="b3bc8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3bc8-107">Methods</span></span>
|<span data-ttu-id="b3bc8-108">Método</span><span class="sxs-lookup"><span data-stu-id="b3bc8-108">Method</span></span>|<span data-ttu-id="b3bc8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3bc8-109">Return Type</span></span>|<span data-ttu-id="b3bc8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3bc8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3bc8-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b3bc8-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b3bc8-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b3bc8-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b3bc8-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b3bc8-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b3bc8-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b3bc8-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b3bc8-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b3bc8-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b3bc8-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b3bc8-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3bc8-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3bc8-117">Properties</span></span>
|<span data-ttu-id="b3bc8-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3bc8-118">Property</span></span>|<span data-ttu-id="b3bc8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3bc8-119">Type</span></span>|<span data-ttu-id="b3bc8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3bc8-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3bc8-121">id</span><span class="sxs-lookup"><span data-stu-id="b3bc8-121">id</span></span>|<span data-ttu-id="b3bc8-122">String</span><span class="sxs-lookup"><span data-stu-id="b3bc8-122">String</span></span>|<span data-ttu-id="b3bc8-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="b3bc8-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b3bc8-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3bc8-124">enrolledDeviceCount</span></span>|<span data-ttu-id="b3bc8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-125">Int32</span></span>|<span data-ttu-id="b3bc8-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="b3bc8-126">Total enrolled device count.</span></span> <span data-ttu-id="b3bc8-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="b3bc8-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b3bc8-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b3bc8-128">mdmEnrolledCount</span></span>|<span data-ttu-id="b3bc8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-129">Int32</span></span>|<span data-ttu-id="b3bc8-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="b3bc8-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b3bc8-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b3bc8-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b3bc8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-132">Int32</span></span>|<span data-ttu-id="b3bc8-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="b3bc8-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b3bc8-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b3bc8-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b3bc8-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b3bc8-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b3bc8-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3bc8-136">Device operating system summary.</span></span>|
|<span data-ttu-id="b3bc8-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3bc8-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b3bc8-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b3bc8-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b3bc8-139">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="b3bc8-139">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3bc8-140">Relações</span><span class="sxs-lookup"><span data-stu-id="b3bc8-140">Relationships</span></span>
<span data-ttu-id="b3bc8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3bc8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3bc8-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3bc8-142">JSON Representation</span></span>
<span data-ttu-id="b3bc8-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3bc8-143">Here is a JSON representation of the resource.</span></span>
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







