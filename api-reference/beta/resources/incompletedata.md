---
author: daspek
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 3abefff4749413648a3f1a56d1dbf6d44f16a471
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496275"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="ce3e0-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="ce3e0-103">incompleteData resource type</span></span>

<span data-ttu-id="ce3e0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce3e0-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce3e0-105">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="ce3e0-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="ce3e0-106">As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="ce3e0-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce3e0-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce3e0-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="ce3e0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce3e0-108">Properties</span></span>

| <span data-ttu-id="ce3e0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce3e0-109">Property</span></span>                  | <span data-ttu-id="ce3e0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce3e0-110">Type</span></span>           | <span data-ttu-id="ce3e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce3e0-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="ce3e0-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="ce3e0-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="ce3e0-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce3e0-113">DateTimeOffset</span></span> | <span data-ttu-id="ce3e0-114">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="ce3e0-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="ce3e0-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="ce3e0-115">wasThrottled</span></span>              | <span data-ttu-id="ce3e0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce3e0-116">Boolean</span></span>        | <span data-ttu-id="ce3e0-117">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="ce3e0-117">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
