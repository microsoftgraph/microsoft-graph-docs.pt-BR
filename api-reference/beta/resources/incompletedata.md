---
author: daspek
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006280"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="d8f8c-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="d8f8c-103">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8f8c-104">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="d8f8c-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="d8f8c-105">As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="d8f8c-105">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8f8c-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8f8c-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="d8f8c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8f8c-107">Properties</span></span>

| <span data-ttu-id="d8f8c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8f8c-108">Property</span></span>                  | <span data-ttu-id="d8f8c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8f8c-109">Type</span></span>           | <span data-ttu-id="d8f8c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8f8c-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="d8f8c-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="d8f8c-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="d8f8c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8f8c-112">DateTimeOffset</span></span> | <span data-ttu-id="d8f8c-113">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d8f8c-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="d8f8c-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="d8f8c-114">wasThrottled</span></span>              | <span data-ttu-id="d8f8c-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8f8c-115">Boolean</span></span>        | <span data-ttu-id="d8f8c-116">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="d8f8c-116">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
