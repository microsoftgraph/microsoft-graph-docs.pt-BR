---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ad327dc26bc9268a5f248206893e3a11e6fb27c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154128"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="f6709-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6709-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="f6709-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6709-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6709-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6709-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6709-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f6709-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="f6709-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6709-107">Properties</span></span>
|<span data-ttu-id="f6709-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6709-108">Property</span></span>|<span data-ttu-id="f6709-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6709-109">Type</span></span>|<span data-ttu-id="f6709-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6709-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6709-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6709-111">allowedDeviceCount</span></span>|<span data-ttu-id="f6709-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f6709-112">Int32</span></span>|<span data-ttu-id="f6709-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="f6709-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="f6709-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6709-114">blockedDeviceCount</span></span>|<span data-ttu-id="f6709-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f6709-115">Int32</span></span>|<span data-ttu-id="f6709-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f6709-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="f6709-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6709-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="f6709-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f6709-118">Int32</span></span>|<span data-ttu-id="f6709-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="f6709-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="f6709-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6709-120">unknownDeviceCount</span></span>|<span data-ttu-id="f6709-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f6709-121">Int32</span></span>|<span data-ttu-id="f6709-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="f6709-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="f6709-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f6709-123">unavailableDeviceCount</span></span>|<span data-ttu-id="f6709-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f6709-124">Int32</span></span>|<span data-ttu-id="f6709-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="f6709-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6709-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f6709-126">Relationships</span></span>
<span data-ttu-id="f6709-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6709-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6709-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6709-128">JSON Representation</span></span>
<span data-ttu-id="f6709-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6709-129">Here is a JSON representation of the resource.</span></span>
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




