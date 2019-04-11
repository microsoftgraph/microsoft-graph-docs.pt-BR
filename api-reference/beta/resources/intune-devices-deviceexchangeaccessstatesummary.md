---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39f944b7559abf72d144f5c1608ec4efec014530
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792437"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="dc4e7-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="dc4e7-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="dc4e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4e7-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dc4e7-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="dc4e7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc4e7-107">Properties</span></span>
|<span data-ttu-id="dc4e7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc4e7-108">Property</span></span>|<span data-ttu-id="dc4e7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc4e7-109">Type</span></span>|<span data-ttu-id="dc4e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc4e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4e7-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc4e7-111">allowedDeviceCount</span></span>|<span data-ttu-id="dc4e7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4e7-112">Int32</span></span>|<span data-ttu-id="dc4e7-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="dc4e7-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc4e7-114">blockedDeviceCount</span></span>|<span data-ttu-id="dc4e7-115">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4e7-115">Int32</span></span>|<span data-ttu-id="dc4e7-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="dc4e7-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc4e7-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="dc4e7-118">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4e7-118">Int32</span></span>|<span data-ttu-id="dc4e7-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="dc4e7-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc4e7-120">unknownDeviceCount</span></span>|<span data-ttu-id="dc4e7-121">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4e7-121">Int32</span></span>|<span data-ttu-id="dc4e7-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="dc4e7-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc4e7-123">unavailableDeviceCount</span></span>|<span data-ttu-id="dc4e7-124">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4e7-124">Int32</span></span>|<span data-ttu-id="dc4e7-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc4e7-126">Relações</span><span class="sxs-lookup"><span data-stu-id="dc4e7-126">Relationships</span></span>
<span data-ttu-id="dc4e7-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dc4e7-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc4e7-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc4e7-128">JSON Representation</span></span>
<span data-ttu-id="dc4e7-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc4e7-129">Here is a JSON representation of the resource.</span></span>
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





