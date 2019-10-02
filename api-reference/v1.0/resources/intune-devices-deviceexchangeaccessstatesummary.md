---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3210643c68a7b5a94bfa3b4f601a2e34efe68e13
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356972"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="5e823-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e823-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="5e823-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e823-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e823-105">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e823-105">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="5e823-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e823-106">Properties</span></span>
|<span data-ttu-id="5e823-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e823-107">Property</span></span>|<span data-ttu-id="5e823-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e823-108">Type</span></span>|<span data-ttu-id="5e823-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e823-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e823-110">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e823-110">allowedDeviceCount</span></span>|<span data-ttu-id="5e823-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5e823-111">Int32</span></span>|<span data-ttu-id="5e823-112">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="5e823-112">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="5e823-113">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e823-113">blockedDeviceCount</span></span>|<span data-ttu-id="5e823-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5e823-114">Int32</span></span>|<span data-ttu-id="5e823-115">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5e823-115">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="5e823-116">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e823-116">quarantinedDeviceCount</span></span>|<span data-ttu-id="5e823-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5e823-117">Int32</span></span>|<span data-ttu-id="5e823-118">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="5e823-118">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="5e823-119">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e823-119">unknownDeviceCount</span></span>|<span data-ttu-id="5e823-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5e823-120">Int32</span></span>|<span data-ttu-id="5e823-121">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5e823-121">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="5e823-122">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5e823-122">unavailableDeviceCount</span></span>|<span data-ttu-id="5e823-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5e823-123">Int32</span></span>|<span data-ttu-id="5e823-124">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="5e823-124">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e823-125">Relações</span><span class="sxs-lookup"><span data-stu-id="5e823-125">Relationships</span></span>
<span data-ttu-id="5e823-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e823-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e823-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e823-127">JSON Representation</span></span>
<span data-ttu-id="5e823-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e823-128">Here is a JSON representation of the resource.</span></span>
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




