---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8ca08b026b8e1cdbac4bd0dc73331a9d5df80fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889982"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="7fb6e-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7fb6e-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="7fb6e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fb6e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fb6e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fb6e-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7fb6e-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="7fb6e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fb6e-108">Properties</span></span>
|<span data-ttu-id="7fb6e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fb6e-109">Property</span></span>|<span data-ttu-id="7fb6e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fb6e-110">Type</span></span>|<span data-ttu-id="7fb6e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fb6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb6e-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fb6e-112">allowedDeviceCount</span></span>|<span data-ttu-id="7fb6e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb6e-113">Int32</span></span>|<span data-ttu-id="7fb6e-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="7fb6e-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fb6e-115">blockedDeviceCount</span></span>|<span data-ttu-id="7fb6e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb6e-116">Int32</span></span>|<span data-ttu-id="7fb6e-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="7fb6e-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fb6e-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="7fb6e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb6e-119">Int32</span></span>|<span data-ttu-id="7fb6e-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="7fb6e-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fb6e-121">unknownDeviceCount</span></span>|<span data-ttu-id="7fb6e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb6e-122">Int32</span></span>|<span data-ttu-id="7fb6e-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="7fb6e-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7fb6e-124">unavailableDeviceCount</span></span>|<span data-ttu-id="7fb6e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7fb6e-125">Int32</span></span>|<span data-ttu-id="7fb6e-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fb6e-127">Relações</span><span class="sxs-lookup"><span data-stu-id="7fb6e-127">Relationships</span></span>
<span data-ttu-id="7fb6e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fb6e-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fb6e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fb6e-129">JSON Representation</span></span>
<span data-ttu-id="7fb6e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fb6e-130">Here is a JSON representation of the resource.</span></span>
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





