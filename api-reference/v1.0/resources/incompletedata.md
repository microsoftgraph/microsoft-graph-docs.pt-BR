---
author: daspek
ms.author: dspektor
title: tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 424a857468473532dc6f2a39c4c13dc94b52406c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054886"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="c5fb5-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="c5fb5-103">incompleteData resource type</span></span>

<span data-ttu-id="c5fb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5fb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5fb5-105">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="c5fb5-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="c5fb5-106">As propriedades dentro podem fornecer informações sobre o motivo pelo qual os dados estão incompletos.</span><span class="sxs-lookup"><span data-stu-id="c5fb5-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="c5fb5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5fb5-107">Properties</span></span>

| <span data-ttu-id="c5fb5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5fb5-108">Property</span></span>                  | <span data-ttu-id="c5fb5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5fb5-109">Type</span></span>           | <span data-ttu-id="c5fb5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5fb5-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="c5fb5-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="c5fb5-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="c5fb5-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5fb5-112">DateTimeOffset</span></span> | <span data-ttu-id="c5fb5-113">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="c5fb5-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="c5fb5-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="c5fb5-114">wasThrottled</span></span>              | <span data-ttu-id="c5fb5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5fb5-115">Boolean</span></span>        | <span data-ttu-id="c5fb5-116">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="c5fb5-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5fb5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5fb5-117">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->

