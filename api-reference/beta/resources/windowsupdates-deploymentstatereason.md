---
title: Tipo de recurso deploymentStateReason
description: Um motivo para um estado de implantação específico.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 19a5063cd4f103b0f065311118bc5d8ac97a3c7a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067826"
---
# <a name="deploymentstatereason-resource-type"></a><span data-ttu-id="05ad1-103">Tipo de recurso deploymentStateReason</span><span class="sxs-lookup"><span data-stu-id="05ad1-103">deploymentStateReason resource type</span></span>

<span data-ttu-id="05ad1-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="05ad1-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05ad1-105">Um motivo para um estado de implantação específico.</span><span class="sxs-lookup"><span data-stu-id="05ad1-105">A reason for a particular deployment state.</span></span>

## <a name="properties"></a><span data-ttu-id="05ad1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05ad1-106">Properties</span></span>
|<span data-ttu-id="05ad1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05ad1-107">Property</span></span>|<span data-ttu-id="05ad1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05ad1-108">Type</span></span>|<span data-ttu-id="05ad1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05ad1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ad1-110">valor</span><span class="sxs-lookup"><span data-stu-id="05ad1-110">value</span></span>|<span data-ttu-id="05ad1-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span><span class="sxs-lookup"><span data-stu-id="05ad1-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span></span>|<span data-ttu-id="05ad1-112">Especifica um motivo para o estado de implantação.</span><span class="sxs-lookup"><span data-stu-id="05ad1-112">Specifies a reason for the deployment state.</span></span> <span data-ttu-id="05ad1-113">Os valores possíveis são: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`.</span><span class="sxs-lookup"><span data-stu-id="05ad1-113">Possible values are: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`.</span></span> <span data-ttu-id="05ad1-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05ad1-114">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05ad1-115">Relações</span><span class="sxs-lookup"><span data-stu-id="05ad1-115">Relationships</span></span>
<span data-ttu-id="05ad1-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05ad1-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05ad1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05ad1-117">JSON representation</span></span>
<span data-ttu-id="05ad1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05ad1-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentStateReason",
  "value": "String"
}
```

