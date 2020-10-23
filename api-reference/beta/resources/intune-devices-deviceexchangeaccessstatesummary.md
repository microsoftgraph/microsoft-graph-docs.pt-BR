---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cd20f76a810f37fde239cb523800d98bd8246700
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728234"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="a391f-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a391f-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="a391f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a391f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a391f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a391f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a391f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a391f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a391f-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a391f-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="a391f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a391f-108">Properties</span></span>
|<span data-ttu-id="a391f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a391f-109">Property</span></span>|<span data-ttu-id="a391f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a391f-110">Type</span></span>|<span data-ttu-id="a391f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a391f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a391f-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a391f-112">allowedDeviceCount</span></span>|<span data-ttu-id="a391f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a391f-113">Int32</span></span>|<span data-ttu-id="a391f-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="a391f-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="a391f-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a391f-115">blockedDeviceCount</span></span>|<span data-ttu-id="a391f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a391f-116">Int32</span></span>|<span data-ttu-id="a391f-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a391f-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="a391f-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a391f-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="a391f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a391f-119">Int32</span></span>|<span data-ttu-id="a391f-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="a391f-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="a391f-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a391f-121">unknownDeviceCount</span></span>|<span data-ttu-id="a391f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a391f-122">Int32</span></span>|<span data-ttu-id="a391f-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="a391f-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="a391f-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a391f-124">unavailableDeviceCount</span></span>|<span data-ttu-id="a391f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a391f-125">Int32</span></span>|<span data-ttu-id="a391f-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="a391f-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a391f-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a391f-127">Relationships</span></span>
<span data-ttu-id="a391f-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a391f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a391f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a391f-129">JSON Representation</span></span>
<span data-ttu-id="a391f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a391f-130">Here is a JSON representation of the resource.</span></span>
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





