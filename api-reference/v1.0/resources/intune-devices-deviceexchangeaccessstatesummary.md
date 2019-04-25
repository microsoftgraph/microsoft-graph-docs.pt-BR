---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c336ee6d4b23983f01a4c4756325960c709194f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541987"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="2c0c9-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2c0c9-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="2c0c9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0c9-105">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c0c9-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="2c0c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c0c9-106">Properties</span></span>
|<span data-ttu-id="2c0c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c0c9-107">Property</span></span>|<span data-ttu-id="2c0c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c0c9-108">Type</span></span>|<span data-ttu-id="2c0c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c0c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0c9-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c0c9-110">allowedDeviceCount</span></span>|<span data-ttu-id="2c0c9-111">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0c9-111">Int32</span></span>|<span data-ttu-id="2c0c9-112">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="2c0c9-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c0c9-113">blockedDeviceCount</span></span>|<span data-ttu-id="2c0c9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0c9-114">Int32</span></span>|<span data-ttu-id="2c0c9-115">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="2c0c9-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c0c9-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="2c0c9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0c9-117">Int32</span></span>|<span data-ttu-id="2c0c9-118">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="2c0c9-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c0c9-119">unknownDeviceCount</span></span>|<span data-ttu-id="2c0c9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0c9-120">Int32</span></span>|<span data-ttu-id="2c0c9-121">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="2c0c9-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2c0c9-122">unavailableDeviceCount</span></span>|<span data-ttu-id="2c0c9-123">Int32</span><span class="sxs-lookup"><span data-stu-id="2c0c9-123">Int32</span></span>|<span data-ttu-id="2c0c9-124">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c0c9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2c0c9-125">Relationships</span></span>
<span data-ttu-id="2c0c9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c0c9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c0c9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c0c9-127">JSON Representation</span></span>
<span data-ttu-id="2c0c9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c0c9-128">Here is a JSON representation of the resource.</span></span>
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



