---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee3f6ddb47025dfc4ff29305f45538cf23bfa8c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754585"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="bc826-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="bc826-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="bc826-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc826-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc826-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc826-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc826-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bc826-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="bc826-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc826-107">Properties</span></span>
|<span data-ttu-id="bc826-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc826-108">Property</span></span>|<span data-ttu-id="bc826-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc826-109">Type</span></span>|<span data-ttu-id="bc826-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc826-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc826-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc826-111">allowedDeviceCount</span></span>|<span data-ttu-id="bc826-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bc826-112">Int32</span></span>|<span data-ttu-id="bc826-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="bc826-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="bc826-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc826-114">blockedDeviceCount</span></span>|<span data-ttu-id="bc826-115">Int32</span><span class="sxs-lookup"><span data-stu-id="bc826-115">Int32</span></span>|<span data-ttu-id="bc826-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc826-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="bc826-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc826-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="bc826-118">Int32</span><span class="sxs-lookup"><span data-stu-id="bc826-118">Int32</span></span>|<span data-ttu-id="bc826-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="bc826-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="bc826-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc826-120">unknownDeviceCount</span></span>|<span data-ttu-id="bc826-121">Int32</span><span class="sxs-lookup"><span data-stu-id="bc826-121">Int32</span></span>|<span data-ttu-id="bc826-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="bc826-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="bc826-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc826-123">unavailableDeviceCount</span></span>|<span data-ttu-id="bc826-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bc826-124">Int32</span></span>|<span data-ttu-id="bc826-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="bc826-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc826-126">Relações</span><span class="sxs-lookup"><span data-stu-id="bc826-126">Relationships</span></span>
<span data-ttu-id="bc826-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bc826-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc826-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc826-128">JSON Representation</span></span>
<span data-ttu-id="bc826-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc826-129">Here is a JSON representation of the resource.</span></span>
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




