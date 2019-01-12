---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 389bba96adc477e90244f6f9800da09ff3e87992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990534"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="70c0a-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="70c0a-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="70c0a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="70c0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70c0a-105">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="70c0a-105">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="70c0a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70c0a-106">Properties</span></span>
|<span data-ttu-id="70c0a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70c0a-107">Property</span></span>|<span data-ttu-id="70c0a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="70c0a-108">Type</span></span>|<span data-ttu-id="70c0a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70c0a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c0a-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70c0a-110">allowedDeviceCount</span></span>|<span data-ttu-id="70c0a-111">Int32</span><span class="sxs-lookup"><span data-stu-id="70c0a-111">Int32</span></span>|<span data-ttu-id="70c0a-112">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="70c0a-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="70c0a-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70c0a-113">blockedDeviceCount</span></span>|<span data-ttu-id="70c0a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="70c0a-114">Int32</span></span>|<span data-ttu-id="70c0a-115">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="70c0a-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="70c0a-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70c0a-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="70c0a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="70c0a-117">Int32</span></span>|<span data-ttu-id="70c0a-118">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="70c0a-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="70c0a-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70c0a-119">unknownDeviceCount</span></span>|<span data-ttu-id="70c0a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="70c0a-120">Int32</span></span>|<span data-ttu-id="70c0a-121">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="70c0a-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="70c0a-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70c0a-122">unavailableDeviceCount</span></span>|<span data-ttu-id="70c0a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="70c0a-123">Int32</span></span>|<span data-ttu-id="70c0a-124">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="70c0a-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c0a-125">Relações</span><span class="sxs-lookup"><span data-stu-id="70c0a-125">Relationships</span></span>
<span data-ttu-id="70c0a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70c0a-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70c0a-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70c0a-127">JSON Representation</span></span>
<span data-ttu-id="70c0a-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70c0a-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



