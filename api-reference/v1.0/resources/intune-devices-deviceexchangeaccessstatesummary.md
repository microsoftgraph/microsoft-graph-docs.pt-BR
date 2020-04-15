---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25bc1fe1592b2aa1a1f0cde1b4bf45b6092a36d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407033"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="05faf-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="05faf-103">deviceExchangeAccessStateSummary resource type</span></span>

<span data-ttu-id="05faf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05faf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05faf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05faf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05faf-106">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="05faf-106">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="05faf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05faf-107">Properties</span></span>
|<span data-ttu-id="05faf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05faf-108">Property</span></span>|<span data-ttu-id="05faf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05faf-109">Type</span></span>|<span data-ttu-id="05faf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05faf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05faf-111">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05faf-111">allowedDeviceCount</span></span>|<span data-ttu-id="05faf-112">Int32</span><span class="sxs-lookup"><span data-stu-id="05faf-112">Int32</span></span>|<span data-ttu-id="05faf-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="05faf-113">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="05faf-114">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05faf-114">blockedDeviceCount</span></span>|<span data-ttu-id="05faf-115">Int32</span><span class="sxs-lookup"><span data-stu-id="05faf-115">Int32</span></span>|<span data-ttu-id="05faf-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05faf-116">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="05faf-117">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05faf-117">quarantinedDeviceCount</span></span>|<span data-ttu-id="05faf-118">Int32</span><span class="sxs-lookup"><span data-stu-id="05faf-118">Int32</span></span>|<span data-ttu-id="05faf-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="05faf-119">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="05faf-120">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05faf-120">unknownDeviceCount</span></span>|<span data-ttu-id="05faf-121">Int32</span><span class="sxs-lookup"><span data-stu-id="05faf-121">Int32</span></span>|<span data-ttu-id="05faf-122">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="05faf-122">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="05faf-123">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="05faf-123">unavailableDeviceCount</span></span>|<span data-ttu-id="05faf-124">Int32</span><span class="sxs-lookup"><span data-stu-id="05faf-124">Int32</span></span>|<span data-ttu-id="05faf-125">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="05faf-125">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05faf-126">Relações</span><span class="sxs-lookup"><span data-stu-id="05faf-126">Relationships</span></span>
<span data-ttu-id="05faf-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05faf-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05faf-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05faf-128">JSON Representation</span></span>
<span data-ttu-id="05faf-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05faf-129">Here is a JSON representation of the resource.</span></span>
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







