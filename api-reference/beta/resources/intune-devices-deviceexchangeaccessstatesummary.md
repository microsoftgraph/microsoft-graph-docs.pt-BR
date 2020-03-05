---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d5116fbe1f2d68a4c24f56e3b77266eafa564f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525107"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="b4b78-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b4b78-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="b4b78-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b4b78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4b78-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4b78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4b78-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4b78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b78-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b4b78-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="b4b78-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4b78-108">Properties</span></span>
|<span data-ttu-id="b4b78-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4b78-109">Property</span></span>|<span data-ttu-id="b4b78-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4b78-110">Type</span></span>|<span data-ttu-id="b4b78-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4b78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4b78-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4b78-112">allowedDeviceCount</span></span>|<span data-ttu-id="b4b78-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b78-113">Int32</span></span>|<span data-ttu-id="b4b78-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="b4b78-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="b4b78-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4b78-115">blockedDeviceCount</span></span>|<span data-ttu-id="b4b78-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b78-116">Int32</span></span>|<span data-ttu-id="b4b78-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b4b78-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="b4b78-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4b78-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="b4b78-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b78-119">Int32</span></span>|<span data-ttu-id="b4b78-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="b4b78-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="b4b78-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4b78-121">unknownDeviceCount</span></span>|<span data-ttu-id="b4b78-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b78-122">Int32</span></span>|<span data-ttu-id="b4b78-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b4b78-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="b4b78-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4b78-124">unavailableDeviceCount</span></span>|<span data-ttu-id="b4b78-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b78-125">Int32</span></span>|<span data-ttu-id="b4b78-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="b4b78-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4b78-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b4b78-127">Relationships</span></span>
<span data-ttu-id="b4b78-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4b78-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4b78-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4b78-129">JSON Representation</span></span>
<span data-ttu-id="b4b78-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4b78-130">Here is a JSON representation of the resource.</span></span>
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



