---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a01a1207801063285d7b59f0fa51c474ae78fb6d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418551"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="d5ceb-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="d5ceb-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="d5ceb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5ceb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5ceb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ceb-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d5ceb-107">Device Exchange Access State summary</span></span>

## <a name="properties"></a><span data-ttu-id="d5ceb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5ceb-108">Properties</span></span>
|<span data-ttu-id="d5ceb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5ceb-109">Property</span></span>|<span data-ttu-id="d5ceb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5ceb-110">Type</span></span>|<span data-ttu-id="d5ceb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5ceb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ceb-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d5ceb-112">allowedDeviceCount</span></span>|<span data-ttu-id="d5ceb-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ceb-113">Int32</span></span>|<span data-ttu-id="d5ceb-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="d5ceb-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d5ceb-115">blockedDeviceCount</span></span>|<span data-ttu-id="d5ceb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ceb-116">Int32</span></span>|<span data-ttu-id="d5ceb-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="d5ceb-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d5ceb-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="d5ceb-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ceb-119">Int32</span></span>|<span data-ttu-id="d5ceb-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="d5ceb-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d5ceb-121">unknownDeviceCount</span></span>|<span data-ttu-id="d5ceb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ceb-122">Int32</span></span>|<span data-ttu-id="d5ceb-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="d5ceb-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d5ceb-124">unavailableDeviceCount</span></span>|<span data-ttu-id="d5ceb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ceb-125">Int32</span></span>|<span data-ttu-id="d5ceb-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5ceb-127">Relações</span><span class="sxs-lookup"><span data-stu-id="d5ceb-127">Relationships</span></span>
<span data-ttu-id="d5ceb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5ceb-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5ceb-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5ceb-129">JSON Representation</span></span>
<span data-ttu-id="d5ceb-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5ceb-130">Here is a JSON representation of the resource.</span></span>
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




