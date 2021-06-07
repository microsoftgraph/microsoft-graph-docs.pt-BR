---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd87163c5e8aff363027ec74eeb060fc23c55fb4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751367"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="56cd2-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56cd2-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="56cd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56cd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56cd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56cd2-106">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="56cd2-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="56cd2-107">Methods</span><span class="sxs-lookup"><span data-stu-id="56cd2-107">Methods</span></span>
|<span data-ttu-id="56cd2-108">Método</span><span class="sxs-lookup"><span data-stu-id="56cd2-108">Method</span></span>|<span data-ttu-id="56cd2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="56cd2-109">Return Type</span></span>|<span data-ttu-id="56cd2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56cd2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56cd2-111">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56cd2-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="56cd2-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56cd2-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="56cd2-113">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56cd2-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="56cd2-114">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56cd2-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="56cd2-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="56cd2-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="56cd2-116">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="56cd2-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56cd2-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56cd2-117">Properties</span></span>
|<span data-ttu-id="56cd2-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56cd2-118">Property</span></span>|<span data-ttu-id="56cd2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="56cd2-119">Type</span></span>|<span data-ttu-id="56cd2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56cd2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56cd2-121">id</span><span class="sxs-lookup"><span data-stu-id="56cd2-121">id</span></span>|<span data-ttu-id="56cd2-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="56cd2-122">String</span></span>|<span data-ttu-id="56cd2-123">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="56cd2-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="56cd2-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56cd2-124">enrolledDeviceCount</span></span>|<span data-ttu-id="56cd2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="56cd2-125">Int32</span></span>|<span data-ttu-id="56cd2-126">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="56cd2-126">Total enrolled device count.</span></span> <span data-ttu-id="56cd2-127">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="56cd2-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="56cd2-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="56cd2-128">mdmEnrolledCount</span></span>|<span data-ttu-id="56cd2-129">Int32</span><span class="sxs-lookup"><span data-stu-id="56cd2-129">Int32</span></span>|<span data-ttu-id="56cd2-130">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="56cd2-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="56cd2-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56cd2-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="56cd2-132">Int32</span><span class="sxs-lookup"><span data-stu-id="56cd2-132">Int32</span></span>|<span data-ttu-id="56cd2-133">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="56cd2-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="56cd2-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="56cd2-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="56cd2-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="56cd2-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="56cd2-136">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56cd2-136">Device operating system summary.</span></span>|
|<span data-ttu-id="56cd2-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="56cd2-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="56cd2-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="56cd2-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="56cd2-139">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="56cd2-139">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="56cd2-140">Relações</span><span class="sxs-lookup"><span data-stu-id="56cd2-140">Relationships</span></span>
<span data-ttu-id="56cd2-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="56cd2-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56cd2-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56cd2-142">JSON Representation</span></span>
<span data-ttu-id="56cd2-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56cd2-143">Here is a JSON representation of the resource.</span></span>
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




