---
author: daspek
ms.author: dspektor
title: tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f26317cf16f0773852df35941c00e88df145cc31
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970615"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="45c26-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="45c26-103">incompleteData resource type</span></span>

<span data-ttu-id="45c26-104">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="45c26-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="45c26-105">As propriedades dentro podem fornecer informações sobre o motivo pelo qual os dados estão incompletos.</span><span class="sxs-lookup"><span data-stu-id="45c26-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="45c26-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45c26-106">Properties</span></span>

| <span data-ttu-id="45c26-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45c26-107">Property</span></span>                  | <span data-ttu-id="45c26-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="45c26-108">Type</span></span>           | <span data-ttu-id="45c26-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="45c26-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="45c26-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="45c26-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="45c26-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45c26-111">DateTimeOffset</span></span> | <span data-ttu-id="45c26-112">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="45c26-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="45c26-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="45c26-113">wasThrottled</span></span>              | <span data-ttu-id="45c26-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="45c26-114">Boolean</span></span>        | <span data-ttu-id="45c26-115">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="45c26-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45c26-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45c26-116">JSON representation</span></span>

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
