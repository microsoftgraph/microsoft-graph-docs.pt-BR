---
title: Tipo de recurso deploymentState
description: Descreve e controla o estado atual de uma implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067229"
---
# <a name="deploymentstate-resource-type"></a><span data-ttu-id="a2817-103">Tipo de recurso deploymentState</span><span class="sxs-lookup"><span data-stu-id="a2817-103">deploymentState resource type</span></span>

<span data-ttu-id="a2817-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a2817-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2817-105">Descreve e controla o estado atual de uma implantação.</span><span class="sxs-lookup"><span data-stu-id="a2817-105">Describes and controls the current state of a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="a2817-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2817-106">Properties</span></span>
|<span data-ttu-id="a2817-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2817-107">Property</span></span>|<span data-ttu-id="a2817-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2817-108">Type</span></span>|<span data-ttu-id="a2817-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2817-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2817-110">reasons</span><span class="sxs-lookup"><span data-stu-id="a2817-110">reasons</span></span>|<span data-ttu-id="a2817-111">[coleção microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)</span><span class="sxs-lookup"><span data-stu-id="a2817-111">[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) collection</span></span>|<span data-ttu-id="a2817-112">Especifica os motivos pelos quais a implantação tem seu valor de estado.</span><span class="sxs-lookup"><span data-stu-id="a2817-112">Specifies the reasons the deployment has its state value.</span></span> <span data-ttu-id="a2817-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2817-113">Read-only.</span></span>|
|<span data-ttu-id="a2817-114">requestedValue</span><span class="sxs-lookup"><span data-stu-id="a2817-114">requestedValue</span></span>|<span data-ttu-id="a2817-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="a2817-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span></span>|<span data-ttu-id="a2817-116">Especifica o estado solicitado da implantação.</span><span class="sxs-lookup"><span data-stu-id="a2817-116">Specifies the requested state of the deployment.</span></span> <span data-ttu-id="a2817-117">Oferece suporte a um subconjunto dos **valores de requestedDeploymentStateValue**.</span><span class="sxs-lookup"><span data-stu-id="a2817-117">Supports a subset of the values for **requestedDeploymentStateValue**.</span></span> <span data-ttu-id="a2817-118">Os valores possíveis são: `none` e `paused`.</span><span class="sxs-lookup"><span data-stu-id="a2817-118">Possible values are: `none`, `paused`.</span></span>|
|<span data-ttu-id="a2817-119">valor</span><span class="sxs-lookup"><span data-stu-id="a2817-119">value</span></span>|<span data-ttu-id="a2817-120">microsoft.graph.windowsUpdates.deploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="a2817-120">microsoft.graph.windowsUpdates.deploymentStateValue</span></span>|<span data-ttu-id="a2817-121">Especifica o estado da implantação.</span><span class="sxs-lookup"><span data-stu-id="a2817-121">Specifies the state of the deployment.</span></span> <span data-ttu-id="a2817-122">Oferece suporte a um subconjunto dos valores **para deploymentStateValue**.</span><span class="sxs-lookup"><span data-stu-id="a2817-122">Supports a subset of the values for **deploymentStateValue**.</span></span> <span data-ttu-id="a2817-123">Os valores possíveis são: `scheduled`, `offering`, `paused`.</span><span class="sxs-lookup"><span data-stu-id="a2817-123">Possible values are: `scheduled`, `offering`, `paused`.</span></span> <span data-ttu-id="a2817-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2817-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2817-125">Relações</span><span class="sxs-lookup"><span data-stu-id="a2817-125">Relationships</span></span>
<span data-ttu-id="a2817-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2817-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2817-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2817-127">JSON representation</span></span>
<span data-ttu-id="a2817-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2817-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

