---
title: Tipo de recurso deviceExchangeAccessStateSummary
description: Resumo do Estado de Acesso ao Exchange do dispositivo
ms.openlocfilehash: fec7290ec559f411bed04e03166b31678d43036f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039828"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="75bd2-103">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="75bd2-103">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="75bd2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75bd2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75bd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75bd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75bd2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="75bd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75bd2-107">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="75bd2-107">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="75bd2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75bd2-108">Properties</span></span>
|<span data-ttu-id="75bd2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75bd2-109">Property</span></span>|<span data-ttu-id="75bd2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75bd2-110">Type</span></span>|<span data-ttu-id="75bd2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75bd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75bd2-112">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75bd2-112">allowedDeviceCount</span></span>|<span data-ttu-id="75bd2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="75bd2-113">Int32</span></span>|<span data-ttu-id="75bd2-114">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="75bd2-114">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="75bd2-115">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75bd2-115">blockedDeviceCount</span></span>|<span data-ttu-id="75bd2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="75bd2-116">Int32</span></span>|<span data-ttu-id="75bd2-117">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="75bd2-117">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="75bd2-118">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75bd2-118">quarantinedDeviceCount</span></span>|<span data-ttu-id="75bd2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="75bd2-119">Int32</span></span>|<span data-ttu-id="75bd2-120">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="75bd2-120">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="75bd2-121">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75bd2-121">unknownDeviceCount</span></span>|<span data-ttu-id="75bd2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="75bd2-122">Int32</span></span>|<span data-ttu-id="75bd2-123">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="75bd2-123">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="75bd2-124">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="75bd2-124">unavailableDeviceCount</span></span>|<span data-ttu-id="75bd2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="75bd2-125">Int32</span></span>|<span data-ttu-id="75bd2-126">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="75bd2-126">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75bd2-127">Relações</span><span class="sxs-lookup"><span data-stu-id="75bd2-127">Relationships</span></span>
<span data-ttu-id="75bd2-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75bd2-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="75bd2-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75bd2-129">JSON Representation</span></span>
<span data-ttu-id="75bd2-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75bd2-130">Here is a JSON representation of the resource.</span></span>
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





