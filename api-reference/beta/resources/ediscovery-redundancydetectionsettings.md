---
title: Tipo de recurso redundancyDetectionSettings
description: Configurações de redundância para um caso de Descoberta e
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fd1ca1ea3faf03e2639896c79acd0629931c71c9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080715"
---
# <a name="redundancydetectionsettings-resource-type"></a><span data-ttu-id="b3e1f-103">Tipo de recurso redundancyDetectionSettings</span><span class="sxs-lookup"><span data-stu-id="b3e1f-103">redundancyDetectionSettings resource type</span></span>

<span data-ttu-id="b3e1f-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b3e1f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e1f-105">Redundância (threading de email e detecção quase duplicada) para um caso de Descoberta Automática.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-105">Redundancy (email threading and near duplicate detection) settings for an eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="b3e1f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3e1f-106">Properties</span></span>

|<span data-ttu-id="b3e1f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3e1f-107">Property</span></span>|<span data-ttu-id="b3e1f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3e1f-108">Type</span></span>|<span data-ttu-id="b3e1f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e1f-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b3e1f-110">isEnabled</span></span>|<span data-ttu-id="b3e1f-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3e1f-111">Boolean</span></span>|<span data-ttu-id="b3e1f-112">Indica se o threading de email e a detecção quase duplicada estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-112">Indicates whether email threading and near duplicate detection are enabled.</span></span>|
|<span data-ttu-id="b3e1f-113">maxWords</span><span class="sxs-lookup"><span data-stu-id="b3e1f-113">maxWords</span></span>|<span data-ttu-id="b3e1f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e1f-114">Int32</span></span>|<span data-ttu-id="b3e1f-115">Consulte [Número mínimo/máximo de palavras para](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) saber mais.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-115">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="b3e1f-116">minWords</span><span class="sxs-lookup"><span data-stu-id="b3e1f-116">minWords</span></span>|<span data-ttu-id="b3e1f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e1f-117">Int32</span></span>|<span data-ttu-id="b3e1f-118">Consulte [Número mínimo/máximo de palavras para](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) saber mais.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-118">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="b3e1f-119">similarityThreshold</span><span class="sxs-lookup"><span data-stu-id="b3e1f-119">similarityThreshold</span></span>|<span data-ttu-id="b3e1f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e1f-120">Int32</span></span>|<span data-ttu-id="b3e1f-121">Consulte [Limite de semelhança de documento e email](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-121">See [Document and email similarity threshold](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3e1f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b3e1f-122">Relationships</span></span>

<span data-ttu-id="b3e1f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3e1f-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3e1f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3e1f-124">JSON representation</span></span>

<span data-ttu-id="b3e1f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3e1f-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
