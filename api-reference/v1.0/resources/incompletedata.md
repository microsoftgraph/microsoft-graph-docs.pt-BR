---
author: daspek
ms.author: dspektor
title: tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029236"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="d67af-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="d67af-103">incompleteData resource type</span></span>

<span data-ttu-id="d67af-104">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="d67af-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="d67af-105">As propriedades dentro podem fornecer informações sobre o motivo pelo qual os dados estão incompletos.</span><span class="sxs-lookup"><span data-stu-id="d67af-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="d67af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d67af-106">Properties</span></span>

| <span data-ttu-id="d67af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d67af-107">Property</span></span>                  | <span data-ttu-id="d67af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d67af-108">Type</span></span>           | <span data-ttu-id="d67af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d67af-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="d67af-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="d67af-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="d67af-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d67af-111">DateTimeOffset</span></span> | <span data-ttu-id="d67af-112">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="d67af-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="d67af-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="d67af-113">wasThrottled</span></span>              | <span data-ttu-id="d67af-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="d67af-114">Boolean</span></span>        | <span data-ttu-id="d67af-115">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="d67af-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d67af-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d67af-116">JSON representation</span></span>

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
