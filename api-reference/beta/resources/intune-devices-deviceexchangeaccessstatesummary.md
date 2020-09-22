---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8466628f74aa3098227c0b7714b86021c7eb6f93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060486"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="7b4c2-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7b4c2-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="7b4c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b4c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b4c2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b4c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b4c2-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7b4c2-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="7b4c2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b4c2-108">Properties</span></span>
|<span data-ttu-id="7b4c2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b4c2-109">Property</span></span>|<span data-ttu-id="7b4c2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b4c2-110">Type</span></span>|<span data-ttu-id="7b4c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b4c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b4c2-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b4c2-112">allowedDeviceCount</span></span>|<span data-ttu-id="7b4c2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7b4c2-113">Int32</span></span>|<span data-ttu-id="7b4c2-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="7b4c2-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b4c2-115">blockedDeviceCount</span></span>|<span data-ttu-id="7b4c2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7b4c2-116">Int32</span></span>|<span data-ttu-id="7b4c2-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="7b4c2-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b4c2-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="7b4c2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7b4c2-119">Int32</span></span>|<span data-ttu-id="7b4c2-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="7b4c2-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b4c2-121">unknownDeviceCount</span></span>|<span data-ttu-id="7b4c2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7b4c2-122">Int32</span></span>|<span data-ttu-id="7b4c2-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="7b4c2-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b4c2-124">unavailableDeviceCount</span></span>|<span data-ttu-id="7b4c2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7b4c2-125">Int32</span></span>|<span data-ttu-id="7b4c2-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b4c2-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7b4c2-127">Relationships</span></span>
<span data-ttu-id="7b4c2-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b4c2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b4c2-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b4c2-129">JSON Representation</span></span>
<span data-ttu-id="7b4c2-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b4c2-130">Here is a JSON representation of the resource.</span></span>
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






