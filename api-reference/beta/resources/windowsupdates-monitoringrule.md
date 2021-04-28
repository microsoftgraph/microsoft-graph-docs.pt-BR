---
title: tipo de recurso monitoringRule
description: Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067793"
---
# <a name="monitoringrule-resource-type"></a><span data-ttu-id="21dcc-103">tipo de recurso monitoringRule</span><span class="sxs-lookup"><span data-stu-id="21dcc-103">monitoringRule resource type</span></span>

<span data-ttu-id="21dcc-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="21dcc-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21dcc-105">Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.</span><span class="sxs-lookup"><span data-stu-id="21dcc-105">Rule defining a signal and threshold to monitor, and the action to perform when met.</span></span>

## <a name="properties"></a><span data-ttu-id="21dcc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21dcc-106">Properties</span></span>
|<span data-ttu-id="21dcc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21dcc-107">Property</span></span>|<span data-ttu-id="21dcc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="21dcc-108">Type</span></span>|<span data-ttu-id="21dcc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="21dcc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21dcc-110">ação</span><span class="sxs-lookup"><span data-stu-id="21dcc-110">action</span></span>|<span data-ttu-id="21dcc-111">microsoft.graph.windowsUpdates.monitoringAction</span><span class="sxs-lookup"><span data-stu-id="21dcc-111">microsoft.graph.windowsUpdates.monitoringAction</span></span>|    <span data-ttu-id="21dcc-112">A ação acionada quando o limite para o sinal determinado é atendido.</span><span class="sxs-lookup"><span data-stu-id="21dcc-112">The action triggered when the threshold for the given signal is met.</span></span> <span data-ttu-id="21dcc-113">Os valores possíveis são: `alertError` e `pauseDeployment`.</span><span class="sxs-lookup"><span data-stu-id="21dcc-113">Possible values are: `alertError`, `pauseDeployment`.</span></span>|
|<span data-ttu-id="21dcc-114">signal</span><span class="sxs-lookup"><span data-stu-id="21dcc-114">signal</span></span>|<span data-ttu-id="21dcc-115">microsoft.graph.windowsUpdates.monitoringSignal</span><span class="sxs-lookup"><span data-stu-id="21dcc-115">microsoft.graph.windowsUpdates.monitoringSignal</span></span>|<span data-ttu-id="21dcc-116">O sinal a ser monitorado.</span><span class="sxs-lookup"><span data-stu-id="21dcc-116">The signal to monitor.</span></span> <span data-ttu-id="21dcc-117">Os valores possíveis são: `rollback` .</span><span class="sxs-lookup"><span data-stu-id="21dcc-117">Possible values are: `rollback`.</span></span>|
|<span data-ttu-id="21dcc-118">threshold</span><span class="sxs-lookup"><span data-stu-id="21dcc-118">threshold</span></span>|<span data-ttu-id="21dcc-119">Int32</span><span class="sxs-lookup"><span data-stu-id="21dcc-119">Int32</span></span>|<span data-ttu-id="21dcc-120">O limite para um sinal no qual disparar a ação.</span><span class="sxs-lookup"><span data-stu-id="21dcc-120">The threshold for a signal at which to trigger action.</span></span> <span data-ttu-id="21dcc-121">Um inteiro de 1 a 100 (inclusive).</span><span class="sxs-lookup"><span data-stu-id="21dcc-121">An integer from 1 to 100 (inclusive).</span></span>|

## <a name="relationships"></a><span data-ttu-id="21dcc-122">Relações</span><span class="sxs-lookup"><span data-stu-id="21dcc-122">Relationships</span></span>
<span data-ttu-id="21dcc-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21dcc-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21dcc-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21dcc-124">JSON representation</span></span>
<span data-ttu-id="21dcc-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21dcc-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

