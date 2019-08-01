---
title: Tipo de recurso managedDeviceOverview
description: Dados de resumo de dispositivos gerenciados
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f10e34f8db0a671463740f0cbf42785c09170286
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030734"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="ff4c0-103">Tipo de recurso managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff4c0-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="ff4c0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff4c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff4c0-105">Dados de resumo de dispositivos gerenciados</span><span class="sxs-lookup"><span data-stu-id="ff4c0-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="ff4c0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff4c0-106">Methods</span></span>
|<span data-ttu-id="ff4c0-107">Método</span><span class="sxs-lookup"><span data-stu-id="ff4c0-107">Method</span></span>|<span data-ttu-id="ff4c0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff4c0-108">Return Type</span></span>|<span data-ttu-id="ff4c0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4c0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff4c0-110">Obter managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff4c0-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="ff4c0-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff4c0-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ff4c0-112">Ler propriedades e relações de objetos de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ff4c0-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="ff4c0-113">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff4c0-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="ff4c0-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff4c0-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ff4c0-115">Atualizar as propriedades de um objeto de [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ff4c0-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff4c0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff4c0-116">Properties</span></span>
|<span data-ttu-id="ff4c0-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff4c0-117">Property</span></span>|<span data-ttu-id="ff4c0-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff4c0-118">Type</span></span>|<span data-ttu-id="ff4c0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4c0-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4c0-120">id</span><span class="sxs-lookup"><span data-stu-id="ff4c0-120">id</span></span>|<span data-ttu-id="ff4c0-121">String</span><span class="sxs-lookup"><span data-stu-id="ff4c0-121">String</span></span>|<span data-ttu-id="ff4c0-122">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="ff4c0-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="ff4c0-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff4c0-123">enrolledDeviceCount</span></span>|<span data-ttu-id="ff4c0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4c0-124">Int32</span></span>|<span data-ttu-id="ff4c0-125">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="ff4c0-125">Total enrolled device count.</span></span> <span data-ttu-id="ff4c0-126">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="ff4c0-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="ff4c0-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="ff4c0-127">mdmEnrolledCount</span></span>|<span data-ttu-id="ff4c0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4c0-128">Int32</span></span>|<span data-ttu-id="ff4c0-129">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="ff4c0-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="ff4c0-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff4c0-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="ff4c0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4c0-131">Int32</span></span>|<span data-ttu-id="ff4c0-132">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="ff4c0-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="ff4c0-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ff4c0-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="ff4c0-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="ff4c0-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="ff4c0-135">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff4c0-135">Device operating system summary.</span></span>|
|<span data-ttu-id="ff4c0-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ff4c0-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="ff4c0-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ff4c0-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="ff4c0-138">Distribuição do estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="ff4c0-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4c0-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ff4c0-139">Relationships</span></span>
<span data-ttu-id="ff4c0-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff4c0-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff4c0-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff4c0-141">JSON Representation</span></span>
<span data-ttu-id="ff4c0-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff4c0-142">Here is a JSON representation of the resource.</span></span>
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



