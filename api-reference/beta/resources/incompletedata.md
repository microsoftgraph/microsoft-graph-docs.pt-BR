---
author: daspek
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6505d02ee7436e02d90627cfd38a83e3e436706a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016554"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="16c84-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="16c84-103">incompleteData resource type</span></span>

<span data-ttu-id="16c84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c84-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16c84-105">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="16c84-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="16c84-106">As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="16c84-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16c84-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16c84-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="16c84-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16c84-108">Properties</span></span>

| <span data-ttu-id="16c84-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16c84-109">Property</span></span>                  | <span data-ttu-id="16c84-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="16c84-110">Type</span></span>           | <span data-ttu-id="16c84-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16c84-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="16c84-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="16c84-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="16c84-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16c84-113">DateTimeOffset</span></span> | <span data-ttu-id="16c84-114">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="16c84-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="16c84-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="16c84-115">wasThrottled</span></span>              | <span data-ttu-id="16c84-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="16c84-116">Boolean</span></span>        | <span data-ttu-id="16c84-117">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="16c84-117">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


