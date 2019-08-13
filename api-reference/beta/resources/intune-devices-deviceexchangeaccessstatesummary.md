---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91f0b831beee100b4c88b23f2a92f2cc0aebbfee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320788"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="59717-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="59717-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="59717-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59717-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59717-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="59717-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="59717-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59717-107">Properties</span></span>
|<span data-ttu-id="59717-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59717-108">Property</span></span>|<span data-ttu-id="59717-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="59717-109">Type</span></span>|<span data-ttu-id="59717-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="59717-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59717-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59717-111">allowedDeviceCount</span></span>|<span data-ttu-id="59717-112">Int32</span><span class="sxs-lookup"><span data-stu-id="59717-112">Int32</span></span>|<span data-ttu-id="59717-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="59717-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="59717-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59717-114">blockedDeviceCount</span></span>|<span data-ttu-id="59717-115">Int32</span><span class="sxs-lookup"><span data-stu-id="59717-115">Int32</span></span>|<span data-ttu-id="59717-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59717-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="59717-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59717-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="59717-118">Int32</span><span class="sxs-lookup"><span data-stu-id="59717-118">Int32</span></span>|<span data-ttu-id="59717-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="59717-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="59717-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59717-120">unknownDeviceCount</span></span>|<span data-ttu-id="59717-121">Int32</span><span class="sxs-lookup"><span data-stu-id="59717-121">Int32</span></span>|<span data-ttu-id="59717-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="59717-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="59717-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="59717-123">unavailableDeviceCount</span></span>|<span data-ttu-id="59717-124">Int32</span><span class="sxs-lookup"><span data-stu-id="59717-124">Int32</span></span>|<span data-ttu-id="59717-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="59717-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59717-126">Relações</span><span class="sxs-lookup"><span data-stu-id="59717-126">Relationships</span></span>
<span data-ttu-id="59717-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59717-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59717-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59717-128">JSON Representation</span></span>
<span data-ttu-id="59717-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59717-129">Here is a JSON representation of the resource.</span></span>
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



