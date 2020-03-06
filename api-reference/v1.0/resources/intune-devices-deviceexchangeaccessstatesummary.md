---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 170717617679a1a2dc05dc0e0f4f617fab78467d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530303"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="ae55e-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="ae55e-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="ae55e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae55e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae55e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae55e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae55e-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ae55e-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="ae55e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae55e-107">Properties</span></span>
|<span data-ttu-id="ae55e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae55e-108">Property</span></span>|<span data-ttu-id="ae55e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae55e-109">Type</span></span>|<span data-ttu-id="ae55e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae55e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae55e-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae55e-111">allowedDeviceCount</span></span>|<span data-ttu-id="ae55e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ae55e-112">Int32</span></span>|<span data-ttu-id="ae55e-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="ae55e-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="ae55e-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae55e-114">blockedDeviceCount</span></span>|<span data-ttu-id="ae55e-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ae55e-115">Int32</span></span>|<span data-ttu-id="ae55e-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ae55e-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="ae55e-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae55e-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="ae55e-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ae55e-118">Int32</span></span>|<span data-ttu-id="ae55e-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="ae55e-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="ae55e-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae55e-120">unknownDeviceCount</span></span>|<span data-ttu-id="ae55e-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ae55e-121">Int32</span></span>|<span data-ttu-id="ae55e-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ae55e-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="ae55e-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae55e-123">unavailableDeviceCount</span></span>|<span data-ttu-id="ae55e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ae55e-124">Int32</span></span>|<span data-ttu-id="ae55e-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="ae55e-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae55e-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ae55e-126">Relationships</span></span>
<span data-ttu-id="ae55e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae55e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae55e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae55e-128">JSON Representation</span></span>
<span data-ttu-id="ae55e-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae55e-129">Here is a JSON representation of the resource.</span></span>
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




