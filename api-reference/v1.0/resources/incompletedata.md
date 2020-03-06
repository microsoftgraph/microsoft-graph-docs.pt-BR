---
author: daspek
ms.author: dspektor
title: tipo de recurso incompleteData
description: A faceta incompleteData indica que um recurso foi gerado com dados incompletos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5fdf78b0fdb0a34e87296619c477d9f868d0756e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531320"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="61cee-103">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="61cee-103">incompleteData resource type</span></span>

<span data-ttu-id="61cee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61cee-105">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="61cee-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="61cee-106">As propriedades dentro podem fornecer informações sobre o motivo pelo qual os dados estão incompletos.</span><span class="sxs-lookup"><span data-stu-id="61cee-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="61cee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61cee-107">Properties</span></span>

| <span data-ttu-id="61cee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61cee-108">Property</span></span>                  | <span data-ttu-id="61cee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="61cee-109">Type</span></span>           | <span data-ttu-id="61cee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cee-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="61cee-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="61cee-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="61cee-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61cee-112">DateTimeOffset</span></span> | <span data-ttu-id="61cee-113">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="61cee-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="61cee-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="61cee-114">wasThrottled</span></span>              | <span data-ttu-id="61cee-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="61cee-115">Boolean</span></span>        | <span data-ttu-id="61cee-116">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="61cee-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61cee-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61cee-117">JSON representation</span></span>

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
