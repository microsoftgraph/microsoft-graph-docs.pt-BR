---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7f26e49217ea43e64e43e9cdd4cce4b88bae561
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785004"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="777e0-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="777e0-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="777e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="777e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="777e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="777e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="777e0-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="777e0-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="777e0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="777e0-107">Properties</span></span>
|<span data-ttu-id="777e0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777e0-108">Property</span></span>|<span data-ttu-id="777e0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="777e0-109">Type</span></span>|<span data-ttu-id="777e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="777e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="777e0-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="777e0-111">allowedDeviceCount</span></span>|<span data-ttu-id="777e0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="777e0-112">Int32</span></span>|<span data-ttu-id="777e0-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="777e0-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="777e0-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="777e0-114">blockedDeviceCount</span></span>|<span data-ttu-id="777e0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="777e0-115">Int32</span></span>|<span data-ttu-id="777e0-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="777e0-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="777e0-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="777e0-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="777e0-118">Int32</span><span class="sxs-lookup"><span data-stu-id="777e0-118">Int32</span></span>|<span data-ttu-id="777e0-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="777e0-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="777e0-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="777e0-120">unknownDeviceCount</span></span>|<span data-ttu-id="777e0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="777e0-121">Int32</span></span>|<span data-ttu-id="777e0-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="777e0-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="777e0-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="777e0-123">unavailableDeviceCount</span></span>|<span data-ttu-id="777e0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="777e0-124">Int32</span></span>|<span data-ttu-id="777e0-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="777e0-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="777e0-126">Relações</span><span class="sxs-lookup"><span data-stu-id="777e0-126">Relationships</span></span>
<span data-ttu-id="777e0-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="777e0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="777e0-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="777e0-128">JSON Representation</span></span>
<span data-ttu-id="777e0-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="777e0-129">Here is a JSON representation of the resource.</span></span>
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



