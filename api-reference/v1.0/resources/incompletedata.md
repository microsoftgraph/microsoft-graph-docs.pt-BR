---
author: daspek
title: Tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 20dda8e9d1cd321a465c7a257cb5cb7bed845351
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239930"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="4eb35-103">Tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="4eb35-103">incompleteData resource type</span></span>

<span data-ttu-id="4eb35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4eb35-105">A **faceta incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="4eb35-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="4eb35-106">As propriedades dentro podem fornecer informações sobre por que os dados estão incompletos.</span><span class="sxs-lookup"><span data-stu-id="4eb35-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="4eb35-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4eb35-107">Properties</span></span>

| <span data-ttu-id="4eb35-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4eb35-108">Property</span></span>                  | <span data-ttu-id="4eb35-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb35-109">Type</span></span>           | <span data-ttu-id="4eb35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb35-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="4eb35-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb35-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="4eb35-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb35-112">DateTimeOffset</span></span> | <span data-ttu-id="4eb35-113">O serviço não tem dados de origem antes da hora especificada.</span><span class="sxs-lookup"><span data-stu-id="4eb35-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="4eb35-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="4eb35-114">wasThrottled</span></span>              | <span data-ttu-id="4eb35-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="4eb35-115">Boolean</span></span>        | <span data-ttu-id="4eb35-116">Alguns dados não foram registrados devido a atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="4eb35-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eb35-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4eb35-117">JSON representation</span></span>

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

