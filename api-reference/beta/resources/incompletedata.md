---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339962"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="18379-102">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="18379-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18379-103">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="18379-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="18379-104">As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="18379-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18379-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18379-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="18379-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18379-106">Properties</span></span>

| <span data-ttu-id="18379-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18379-107">Property</span></span>                  | <span data-ttu-id="18379-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="18379-108">Type</span></span>           | <span data-ttu-id="18379-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18379-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="18379-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="18379-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="18379-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18379-111">DateTimeOffset</span></span> | <span data-ttu-id="18379-112">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="18379-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="18379-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="18379-113">wasThrottled</span></span>              | <span data-ttu-id="18379-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="18379-114">Boolean</span></span>        | <span data-ttu-id="18379-115">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="18379-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
