---
title: Tipo de recurso rolloutSettings
description: Configurações controlar como o serviço implanta uma atualização ao longo do tempo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 705eeae189d9159c07d3c115c77383a207eae6db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067789"
---
# <a name="rolloutsettings-resource-type"></a><span data-ttu-id="74005-103">Tipo de recurso rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="74005-103">rolloutSettings resource type</span></span>

<span data-ttu-id="74005-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="74005-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74005-105">Configurações controlar como o serviço implanta uma atualização ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="74005-105">Settings controlling how the service deploys an update over time.</span></span>

## <a name="properties"></a><span data-ttu-id="74005-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74005-106">Properties</span></span>
|<span data-ttu-id="74005-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74005-107">Property</span></span>|<span data-ttu-id="74005-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="74005-108">Type</span></span>|<span data-ttu-id="74005-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74005-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74005-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="74005-110">startDateTime</span></span>|<span data-ttu-id="74005-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74005-111">DateTimeOffset</span></span>|<span data-ttu-id="74005-112">Data em que dispositivos na implantação começam a receber a atualização.</span><span class="sxs-lookup"><span data-stu-id="74005-112">Date on which devices in the deployment start receiving the update.</span></span> <span data-ttu-id="74005-113">Quando não estiver definida, a implantação será iniciada assim que os dispositivos são atribuídos.</span><span class="sxs-lookup"><span data-stu-id="74005-113">When not set, the deployment starts as soon as devices are assigned.</span></span>|
|<span data-ttu-id="74005-114">devicesPerOffer</span><span class="sxs-lookup"><span data-stu-id="74005-114">devicesPerOffer</span></span>|<span data-ttu-id="74005-115">Int32</span><span class="sxs-lookup"><span data-stu-id="74005-115">Int32</span></span>| <span data-ttu-id="74005-116">Especifica o número de dispositivos oferecidos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="74005-116">Specifies the number of devices that are offered at the same time.</span></span> <span data-ttu-id="74005-117">Não tem efeito quando **endDateTime** é definido.</span><span class="sxs-lookup"><span data-stu-id="74005-117">Has no effect when **endDateTime** is set.</span></span> <span data-ttu-id="74005-118">Quando **endDateTime** e **devicesPerOffer** não estão definidos, todos os dispositivos na implantação são oferecidos conteúdo ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="74005-118">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|
|<span data-ttu-id="74005-119">durationBetweenOffers</span><span class="sxs-lookup"><span data-stu-id="74005-119">durationBetweenOffers</span></span>|<span data-ttu-id="74005-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74005-120">String</span></span>|<span data-ttu-id="74005-121">Especifica a duração entre cada conjunto de dispositivos que estão sendo oferecidos a atualização.</span><span class="sxs-lookup"><span data-stu-id="74005-121">Specifies duration between each set of devices being offered the update.</span></span> <span data-ttu-id="74005-122">Tem efeito quando **endDateTime** ou **devicesPerOffer** são definidos.</span><span class="sxs-lookup"><span data-stu-id="74005-122">Has an effect when **endDateTime** or **devicesPerOffer** are defined.</span></span> <span data-ttu-id="74005-123">O valor padrão `P1D` é (1 dia).</span><span class="sxs-lookup"><span data-stu-id="74005-123">Default value is `P1D` (1 day).</span></span>|
|<span data-ttu-id="74005-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="74005-124">endDateTime</span></span>|<span data-ttu-id="74005-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74005-125">DateTimeOffset</span></span>|<span data-ttu-id="74005-126">Especifica a data anterior à qual todos os dispositivos atualmente na implantação são oferecidos a atualização.</span><span class="sxs-lookup"><span data-stu-id="74005-126">Specifies the date before which all devices currently in the deployment are offered the update.</span></span> <span data-ttu-id="74005-127">Os dispositivos adicionados após essa data são oferecidos imediatamente.</span><span class="sxs-lookup"><span data-stu-id="74005-127">Devices added after this date are offered immediately.</span></span> <span data-ttu-id="74005-128">Quando **endDateTime** e **devicesPerOffer** não estão definidos, todos os dispositivos na implantação são oferecidos conteúdo ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="74005-128">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74005-129">Relações</span><span class="sxs-lookup"><span data-stu-id="74005-129">Relationships</span></span>
<span data-ttu-id="74005-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74005-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74005-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74005-131">JSON representation</span></span>
<span data-ttu-id="74005-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74005-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```

