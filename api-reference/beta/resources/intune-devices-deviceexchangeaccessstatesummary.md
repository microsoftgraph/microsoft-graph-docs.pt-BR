---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49afbb3383035711bc950a9a7226a354ae78f0e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920426"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="3c55b-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="3c55b-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="3c55b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c55b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c55b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c55b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c55b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3c55b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c55b-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3c55b-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="3c55b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c55b-108">Properties</span></span>
|<span data-ttu-id="3c55b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c55b-109">Property</span></span>|<span data-ttu-id="3c55b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c55b-110">Type</span></span>|<span data-ttu-id="3c55b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c55b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c55b-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c55b-112">allowedDeviceCount</span></span>|<span data-ttu-id="3c55b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3c55b-113">Int32</span></span>|<span data-ttu-id="3c55b-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="3c55b-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="3c55b-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c55b-115">blockedDeviceCount</span></span>|<span data-ttu-id="3c55b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3c55b-116">Int32</span></span>|<span data-ttu-id="3c55b-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3c55b-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="3c55b-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c55b-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="3c55b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3c55b-119">Int32</span></span>|<span data-ttu-id="3c55b-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="3c55b-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="3c55b-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c55b-121">unknownDeviceCount</span></span>|<span data-ttu-id="3c55b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3c55b-122">Int32</span></span>|<span data-ttu-id="3c55b-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="3c55b-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="3c55b-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3c55b-124">unavailableDeviceCount</span></span>|<span data-ttu-id="3c55b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3c55b-125">Int32</span></span>|<span data-ttu-id="3c55b-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="3c55b-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c55b-127">Relações</span><span class="sxs-lookup"><span data-stu-id="3c55b-127">Relationships</span></span>
<span data-ttu-id="3c55b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c55b-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c55b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c55b-129">JSON Representation</span></span>
<span data-ttu-id="3c55b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c55b-130">Here is a JSON representation of the resource.</span></span>
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





